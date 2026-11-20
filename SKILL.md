---
name: action-ledger
trigger: Use in the same turn as any action that changes a file outside the calendar.
---

# Action ledger

Record each action in the ledger, so that the record survives a compaction.

## Procedure

1. After the action, add one row to the ledger: time (local), session id, action, evidence, status.
2. Status is DONE (verified), ATTEMPTED (result not verified), or FAILED.
3. If you find an action that is not in the ledger, add it with its source and say it was backfilled, as the ledger does for its backfilled rows.

## Never

- Never record an action as done because you intended it.

## Checks

- Every change made this turn has a row.

Source: summoner's ledger rule (line 3 of the ledger file), 2026-11-20 (topic: ledger). Status: draft, not published.
