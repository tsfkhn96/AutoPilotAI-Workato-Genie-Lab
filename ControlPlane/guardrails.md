# Guardrails

## Purpose
Keep the agent safe and enterprise-ready.

## Guardrails
- Never execute destructive actions without explicit approval (e.g., terminate user, revoke access org-wide)
- Require structured outputs (JSON) from AI steps
- Validate required fields (name, dates, department, software)
- If confidence is low -> escalate to a human queue (Slack/ServiceNow)

## Escalation Pattern
When missing or ambiguous info:
- Ask follow-up question (if interactive channel)
- OR create a ServiceNow ticket with context
- OR post to Slack with the draft action plan
