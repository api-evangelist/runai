---
name: Submit and manage a training workload
description: Authenticate to NVIDIA Run:ai, submit a training workload to a project, then monitor, suspend/resume, and delete it.
api: openapi/runai-openapi-original.json
operations: [create_training1, get_training, suspend_training, resume_training, delete_training]
---

# Submit and manage a training workload

Use this skill to run a distributed/single-node training job on the NVIDIA Run:ai
control plane and manage its lifecycle.

## Prerequisites
- An access key (clientId + clientSecret) for a user or service account with rights on the target project.
- The `projectId` and `clusterId` you will submit into.
- The base API host: `https://app.run.ai` (SaaS) or your tenant/self-hosted control-plane URL.

## Authentication
1. Request a bearer token: `POST /api/v1/token` with body
   `{"grantType":"client_credentials","clientId":"<ID>","clientSecret":"<SECRET>"}`.
2. Read `accessToken` from the response and send `Authorization: Bearer <accessToken>`
   on every subsequent request. All bodies are `application/json`.

## Steps
1. **Submit the training** — `create_training1` (`POST /api/v1/workloads/trainings`).
   Provide the project/cluster scope and the workload spec (image, compute, environment).
   Capture the returned `workloadId`.
2. **Monitor status** — `get_training` (`GET /api/v1/workloads/trainings/{workloadId}`).
   Poll until the phase reaches Running/Completed.
3. **Pause when needed** — `suspend_training`
   (`POST /api/v1/workloads/trainings/{workloadId}/suspend`) to release GPUs;
   `resume_training` (`POST /api/v1/workloads/trainings/{workloadId}/resume`) to continue.
4. **Clean up** — `delete_training` (`DELETE /api/v1/workloads/trainings/{workloadId}`).

## Conventions and error handling
- Errors return a JSON envelope `{code, message, details?}` (not RFC 9457). Handle 401
  (token expired — re-request), 403 (not authorized for the project), 404 (unknown
  workloadId), and 409 (state conflict, e.g. suspending a non-running workload).
- List endpoints use offset/limit pagination (`limit` default 50, max 500) with a `next` pointer.
