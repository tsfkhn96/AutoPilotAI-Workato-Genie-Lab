# HR ➜ IT Orchestration Chain

This pattern demonstrates how Genies collaborate automatically.

## Scenario

Prompt to HR Genie:
"Onboard Jane Smith as Senior Data Analyst starting Feb 12"

## HR Genie Executes

1. Create employee profile in HRIS / payroll  
2. Trigger background check & I-9 workflow  
3. Provision Okta identity & baseline apps  
4. Generate IT onboarding event

## IT Genie Automatically Invoked

The HR Genie emits the following event:

{
  "event": "new_employee_onboarded",
  "employee": "Jane Smith",
  "role": "Senior Data Analyst",
  "start_date": "2026-02-12"
}

## IT Genie Consumes Event

Actions:
- Create ServiceNow onboarding ticket  
- Assign standard laptop bundle  
- Install role-based software set  
- Notify hiring manager & IT queue  

## Outcome

A single HR prompt now executes two domain Genies seamlessly — illustrating autonomous, cross-department orchestration.
