# Scenario: one backend unavailable

1. Confirm the staging proxy and at least two disposable backends are healthy.
2. Drain the target backend using the documented operator control.
3. Verify new admissions avoid the target and existing sessions receive the documented behavior.
4. Confirm alerts identify the backend and do not trigger an uncontrolled restart loop.
5. Restore the backend, verify readiness, and re-enable it gradually.
6. Record detection, player-visible impact, recovery, and any routing inconsistency.
