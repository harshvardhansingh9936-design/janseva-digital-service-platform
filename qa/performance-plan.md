# Performance Test Plan — Week 3

## Objective
Define measurable performance tests for the JanSeva platform once a staging backend is available.

## Proposed scenarios
| Scenario | Load model | Primary measurements | Proposed pass target |
|---|---|---|---|
| Baseline | 25 concurrent users | p50/p95 response time, error rate | p95 ≤ 2 s for normal interactive requests; error rate < 1% |
| Expected peak | 100 concurrent users | p95 response time, throughput, errors | p95 ≤ 3 s; error rate < 2% |
| Stress | Increase load in controlled steps beyond expected peak | saturation point, errors, recovery | No uncontrolled crash; service recovers after load returns to normal |
| Soak | Sustained expected load | memory/CPU trend, errors | No progressive resource exhaustion or sustained error growth |
| Spike | Rapid increase and decrease in traffic | queueing, recovery, error rate | Graceful degradation and recovery without data corruption |

These are **proposed test thresholds**, not measured results for the current static prototype.

## Workload focus
- Service catalogue/search
- Application submission
- Document upload initiation
- Status queries
- Officer case queries
- Notification processing

## Evidence to collect later
- Test tool configuration
- Concurrent-user profile
- Response-time percentiles
- Throughput
- HTTP error rate
- CPU/memory/database utilisation
- Bottleneck observations
- Recovery time after stress/spike

## Tools
k6 or Apache JMeter are recommended for the staging performance cycle.
