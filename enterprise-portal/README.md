# AXME Cloud Enterprise Portal (Reference Skeleton)

This folder tracks the reference client contract for enterprise admin flows in Track F.

## Alpha Status

> AXME is currently in Alpha.  
> Protocol and API surface are stabilizing and may change.  
> Usage limits apply.  
> Not recommended for production workloads yet.  
> We welcome early adopters and protocol feedback.

## Scope

- organization/workspace bootstrap and administration
- access-request review and approval workflow
- role-aware portal navigation and action gating
- personal cabinet self-service overview
- quota and usage visibility (`summary`, `timeseries`, `rollups`)
- service-account and credential-key lifecycle operations

## API Surface

- `GET /v1/portal/enterprise/navigation`
- `GET /v1/portal/enterprise/overview`
- `GET /v1/portal/enterprise/access-requests`
- `GET /v1/portal/enterprise/request-queue`
- `GET /v1/portal/personal/overview`
- `POST /v1/organizations`
- `POST /v1/organizations/{org_id}/workspaces`
- `POST /v1/access-requests/{access_request_id}/review`
- `GET /v1/quotas`, `PATCH /v1/quotas`
- `GET /v1/usage/summary`, `GET /v1/usage/timeseries`, `POST /v1/usage/rollups/daily`
- `POST /v1/service-accounts`
- `POST /v1/service-accounts/{service_account_id}/keys`
- `POST /v1/service-accounts/{service_account_id}/keys/{key_id}/revoke`

## Notes

- this is a reference integration skeleton (not a production UI package)
- canonical contracts are defined in `axp-spec` and validated in `axp-conformance`
