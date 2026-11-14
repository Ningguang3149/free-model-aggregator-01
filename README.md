# free-model-aggregator-01: Lookahead CSP Constraint Aggregator V2

Deterministic AI Model Aggregator submitted by `@ningguang3149` for the `free-model-aggregator-01` challenge ($500 pot).

## Strategy Overview
- **Solver**: `LookaheadCspRouter` (Forward-Checking Constraint Satisfaction)
- **Architecture**: Forward-checking remaining workload manifest demands against provider specialized capabilities
- **Wire Support**: Dual-wire OpenAI Chat Completions (`/v1/chat/completions`) & Anthropic Messages (`/v1/messages`), supporting JSON and streaming SSE.
- **Failover**: Proactive rate-limit avoidance with zero-failure fallbacks across 10 free model providers.
