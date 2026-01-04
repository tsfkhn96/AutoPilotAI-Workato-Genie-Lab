# Policy Engine

## Purpose
Applies governance before execution:
- Who is allowed to request what?
- What needs approval?
- What should be logged/audited?

## Example Policies

### IT
- Installing licensed software (Adobe, MS Project) requires manager approval.
- Admin access requires Security approval.
- Unknown software names -> escalate to IT queue.

### HR
- Onboarding requires HR approval if start date is within 3 business days.
- Termination requests always require HR + Security approval.

### Sales
- Creating an opportunity > $250K requires Sales Ops approval.
- Duplicate account risk -> run dedupe check before create.
