---
name: Provision a department and project with GPU quota
description: Create an organizational department and a project scoped to a cluster so teams can submit GPU workloads under quota.
api: openapi/runai-openapi-original.json
operations: [create_department, create_project, get_projects]
---

# Provision a department and project with GPU quota

Use this skill to set up the organizational scope (department + project) that
workloads are submitted into on NVIDIA Run:ai.

## Prerequisites
- An access key for a user/service account with administrative rights.
- The target `clusterId`.
- Base API host `https://app.run.ai` (SaaS) or your tenant control-plane URL.

## Authentication
Obtain a bearer token via `POST /api/v1/token` (grantType `client_credentials`) and
send `Authorization: Bearer <accessToken>` on every request.

## Steps
1. **Create the department** — `create_department`
   (`POST /api/v1/org-unit/departments`). Set the department name, the parent
   `clusterId`, and its GPU/CPU/memory resource quota. Capture the department id.
2. **Create the project** — `create_project` (`POST /api/v1/org-unit/projects`).
   Reference the department, set the project quota (deserved/limit GPUs), and
   scheduling policy. Capture the `projectId`.
3. **Verify** — `get_projects` (`GET /api/v1/org-unit/projects`). Confirm the new
   project appears; use `filterBy`, `search`, `sortBy`/`sortOrder`, and offset/limit
   pagination to locate it in large tenants.

## Conventions and error handling
- JSON envelope errors `{code, message, details?}`. Expect 400 (invalid quota/name),
  403 (insufficient rights), 409 (name conflict).
- Some legacy project/department endpoints are deprecated (47 deprecated operations
  in the spec); prefer the `org-unit` operations above.
