# AutoPilotAI – Policy Engine

The Policy Engine acts as a control layer across all genies.

Before any action is executed, policies are evaluated to ensure
security, compliance, and business rules are enforced.

---

## Example Policy Types

| Domain | Policy |
|-------|-------|
| HR | Only HR Managers can trigger employee onboarding |
| IT | Finance software requires VP approval |
| Sales | Opportunities over $100K require Sales Director review |

---

## Example Enforcement Flow

### Prompt

> “Install Bloomberg Terminal for John Doe”

### Policy Evaluation

| Rule | Result |
|------|--------|
| User role is Finance VP? | ❌ No |
| Request contains restricted software? | ✅ Yes |

### Outcome

The IT Genie halts execution and triggers approval workflow:

```json
{
  "status": "blocked",
  "reason": "Restricted software requires Finance VP approval"
}
