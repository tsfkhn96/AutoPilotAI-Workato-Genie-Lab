# Employee Onboarding – Approval Flow

## Trigger
Prompt:
"Onboard Jane Smith as Senior Data Analyst starting Feb 12"

## Policy Evaluation
- Start date < 5 business days → Approval required
- Job role contains privileged access → Security review required

## Approval Flow
1. Slack approval → HR Manager
2. If approved → Slack approval → Security

## Execution
- Create ADP employee
- Provision Okta, Email, Role Apps
- Create IT hardware ticket

## Audit
All actions logged to HR audit table
