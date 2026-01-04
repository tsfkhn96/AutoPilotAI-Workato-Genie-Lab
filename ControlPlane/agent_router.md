# Agent Router

## Purpose
Routes an incoming natural-language request to the correct Genie:
- IT (software provisioning, access requests)
- HR (hire-to-retire lifecycle)
- Sales (lead-to-opportunity automation)

## Input
A single prompt from a user.

## Output
A routing decision:
- domain: IT | HR | SALES
- intent: (domain-specific)
- confidence: 0–1
- requires_approval: true/false

## Example
Prompt:
"Onboard Jane Smith as Senior Data Analyst starting Feb 12"

Decision:
- domain: HR
- intent: employee_onboarding
- confidence: high
- requires_approval: true (creates employee record + access)
