# BASE RULES

## Stack Discovery (Mandatory)
1) Backend language/framework + version
2) DB type + migration tool
3) Auth method + roles
4) Deployment method
5) OpenAPI location (contracts/openapi.yaml)
6) Logging/metrics requirements
7) Expected load + critical operations

## Architecture Principles
- Controller → Service → Repository
- Contract-first API
- DB enforces invariants
- Middleware handles cross-cutting concerns
- Clean, small modules

## Performance Default
- Pagination required
- Indexed queries
- Avoid N+1
- Short transactions
- Scaling path if load grows 10x

## Security Default
- Validate inputs
- Password hash only
- No secrets in logs
- Safe error responses
- Least privilege DB users
