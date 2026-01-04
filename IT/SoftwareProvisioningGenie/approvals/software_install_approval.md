# Software Install – Approval Flow

## Trigger
User prompt:
"Install Adobe Acrobat for John Doe"

## Policy Evaluation
- Is software licensed? → Yes → Approval required
- Is requester manager of employee? → Yes → proceed

## Approval Flow
1. Create Slack approval card to IT Manager
2. Include:
   - User
   - Software
   - License cost
   - Target device

## Outcomes
| Decision | Action |
|-------|--------|
| Approved | Execute installer via endpoint mgmt |
| Rejected | Notify requester with reason |
| Timeout (24h) | Escalate to IT queue |
