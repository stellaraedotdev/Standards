# Performance Guidelines

## Purpose
Provide a repeatable approach for building performant systems and preventing regressions.

## Scope
Applies to backend services, frontend applications, data pipelines, APIs, and infrastructure workloads.

## Performance Principles
- Measure before optimizing.
- Optimize for user-perceived latency and system throughput.
- Prioritize fixes by business impact and frequency.
- Keep solutions simple and observable.

## Budgeting and Targets
- Define service-level objectives and key performance indicators.
- Establish latency, throughput, and resource budgets per system.
- Track p50, p95, and p99 metrics where applicable.

## Development Practices
- Avoid unnecessary allocations, I/O, and round trips.
- Use caching intentionally with clear invalidation strategies.
- Batch or parallelize independent operations where safe.
- Select data structures and algorithms appropriate to scale.

## Data and Storage
- Design queries and indexes to match access patterns.
- Minimize over-fetching and under-fetching.
- Use pagination and streaming for large datasets.

## Frontend Performance
- Minimize critical render path size and complexity.
- Defer non-critical resources and work.
- Optimize assets, caching, and network usage.
- Monitor real user metrics in production.

## Testing and Regression Prevention
- Add benchmark or performance tests for critical paths.
- Track performance metrics in CI where feasible.
- Fail releases when agreed performance budgets are exceeded.

## Observability and Tuning
- Instrument key code paths and dependencies.
- Use profiling tools to identify real bottlenecks.
- Reassess tuning after major architecture changes.

## Rule Severity
- MUST: Required for systems with defined performance budgets.
- SHOULD: Strong recommendations for stable scalability.
- MAY: Optional optimizations after measurement.

## Pull Request Checklist
- Performance impact was assessed.
- Budgets and targets remain within thresholds.
- Benchmarks or metrics were updated when needed.
- Rollout and monitoring plans cover high-risk changes.

<sub>&copy; 2026 Stellarae | Documents licensed under MIT License. Treat the documents outlined here as 'the Software' in terms of the license.</sub>
