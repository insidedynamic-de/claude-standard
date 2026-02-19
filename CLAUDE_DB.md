# DATABASE RULES

- Compatible with PostgreSQL & MySQL unless fixed
- tenant_id-ready schema
- UNIQUE(tenant_id, key)

DB enforces:
- Constraints
- Timestamps
- row_version

Triggers for:
- users
- licenses
- orders

Rules:
- Short, deterministic
- No external calls
- Diff only
