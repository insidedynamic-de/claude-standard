# TELEPHONY / ESL PROFILE

- Explicit concurrency model
- Prefer single event loop
- No shared mutable state

Reliability:
- Timeouts
- Retry idempotent ops
- Circuit breaker
- Reconnection strategy

Observability:
- trace_id + call_id
- Metrics for latency & failures
