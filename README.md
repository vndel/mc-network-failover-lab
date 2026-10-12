# Minecraft Network Failover Lab

Controlled staging exercises for validating how a Minecraft network behaves when a proxy backend, shared dependency, or host becomes unavailable. Do not run these fault injections against production without a separately approved change and tested rollback.

## Exercise guardrails
- Use an isolated environment with synthetic accounts and disposable world data.
- Define blast radius, stop conditions, an exercise lead, and rollback before introducing a fault.
- Change one failure mode at a time and keep player-facing services out of scope.
- Confirm monitoring detects the fault and the operator can restore normal service.
- Capture sanitized timestamps, symptoms, detection delay, recovery time, and lessons.

A failover design is only validated for the conditions actually tested. Repeat after material topology changes.