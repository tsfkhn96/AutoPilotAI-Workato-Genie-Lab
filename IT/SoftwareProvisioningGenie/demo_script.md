# Software Provisioning Genie – Demo Script

This script explains how to demonstrate the Genie during an interview or demo.

---

## 🎬 Scenario

An employee needs Adobe Acrobat installed on their laptop.

User types in Workato Go:

> "Install Adobe Acrobat on my laptop"

---

## 🔄 Genie Execution Flow

| Step | Action |
|------|--------|
| 1 | Genie receives user intent |
| 2 | Detects intent: `software_install` |
| 3 | Validates entitlement policy |
| 4 | Triggers Workato recipe to create ServiceNow request |
| 5 | Calls Intune / Jamf to install software |
| 6 | Sends confirmation to Slack |
| 7 | Closes the ServiceNow ticket |

---

## 📊 Business Outcome

- Zero manual IT intervention  
- Installation completed in minutes  
- Full audit trail maintained
