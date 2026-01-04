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
