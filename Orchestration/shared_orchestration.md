# AutoPilotAI – Shared Orchestration Layer

This layer routes every natural-language prompt to the correct Genie
based on detected business intent.

---

## Unified Entry Point

All genies are invoked through a single control API.

Example:

POST /genie/execute
{
"user": "manager@company.com
",
"message": "Onboard Jane Smith as Senior Data Analyst starting Feb 12"
}


---

## Intent Routing

| Detected Intent | Routed Genie |
|-----------------|--------------|
| software_install | IT – Software Provisioning Genie |
| employee_onboarding | HR – Hire-to-Retire Genie |
| create_opportunity | Sales – Lead-to-Opportunity Genie |

---

## Execution Lifecycle

1. Prompt received by Control Plane
2. AI extracts intent & entities
3. Policy Engine evaluates permissions
4. Genie-specific workflow is invoked
5. Execution status is streamed back to user
6. Audit trail is recorded

---

## Sample Router Output

```json
{
  "intent": "employee_onboarding",
  "genie": "HR-HireToRetire",
  "status": "accepted",
  "execution_id": "HR-2026-00091"
}
