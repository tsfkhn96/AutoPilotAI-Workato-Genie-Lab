# AutoPilotAI – Human-in-the-Loop Approval Framework

Not every AI action should be executed automatically.

This framework enforces approval gates based on risk level.

---

## Approval Classification

| Intent | Risk Level | Approval Required |
|--------|------------|------------------|
| software_install | Low | No |
| employee_onboarding | Medium | HR Manager |
| terminate_employee | High | HR Director + IT Security |
| delete_customer_data | Critical | Legal + Security |

---

## Example – HR Termination Request

**Prompt**
"Terminate employee John Smith effective immediately."


---

## Approval Flow

1. AI detects intent: `terminate_employee`
2. System pauses execution
3. Approval request sent to:
   - HR Director
   - IT Security Lead
4. Once approvals received:
   - Okta access revoked
   - Payroll deactivated
   - Assets flagged for recovery
   - Audit record finalized

---

## Approval Payload

```json
{
  "intent": "terminate_employee",
  "requested_by": "manager@company.com",
  "approvers": ["hr.director@company.com", "it.security@company.com"],
  "status": "pending"
}
