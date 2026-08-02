---
name: Launch an interactive workspace
description: Launch an interactive GPU workspace (e.g. Jupyter/VS Code) on NVIDIA Run:ai and find it in the workloads list.
api: openapi/runai-openapi-original.json
operations: [create_workspace1, get_workloads]
---

# Launch an interactive workspace

Use this skill to give a researcher an interactive, GPU-backed development
environment on NVIDIA Run:ai.

## Prerequisites
- An access key for a user/service account with rights on the target project.
- The `projectId` and `clusterId`, plus the environment/compute assets to attach.
- Base API host `https://app.run.ai` (SaaS) or your tenant control-plane URL.

## Authentication
Get a bearer token from `POST /api/v1/token` (grantType `client_credentials`) and
send `Authorization: Bearer <accessToken>` on every request.

## Steps
1. **Create the workspace** — `create_workspace1`
   (`POST /api/v1/workloads/workspaces`). Provide the project/cluster scope and the
   workspace spec (image or environment asset, compute asset, data sources,
   connections/ports). Capture the returned `workloadId`.
2. **Locate it** — `get_workloads` (`GET /api/v1/workloads`). Filter to your
   workspace with `filterBy` (e.g. `type==Workspace`), `search`, and offset/limit
   pagination; read its status and the connection URL for the researcher.

## Conventions and error handling
- Errors are a JSON envelope `{code, message, details?}`. Handle 401 (expired token),
  403 (project access), 404, and 409 (state conflict).
- The workloads list supports `sortBy`/`sortOrder`, `filterBy` operators
  (`==`, `!=`, `>=`, `=@`), free-text `search`, and a `next` pagination pointer.
