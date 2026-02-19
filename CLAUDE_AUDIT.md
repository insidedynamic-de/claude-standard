# AUDIT POLICY

Log security events:
- LOGIN_SUCCESS / FAILED
- LOGOUT
- TOKEN_REFRESH

Log data changes:
- INSERT / UPDATE / DELETE
- Store diff only

Context:
- actor_id
- action
- entity
- trace_id

RBAC:
- superadmin: full + revert
- support: read-only

Retention:
- IP/User-Agent 180 days (configurable)

Revert:
- superadmin only
- New transaction
- Logs REVERT action
