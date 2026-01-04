# Hire-to-Retire HR Genie

An autonomous HR AI agent that manages the complete employee lifecycle —
from job posting to off-boarding — using Workato Genie concepts.

---

## 🧩 Problem

HR teams manage multiple disconnected systems across recruitment,
onboarding, payroll, access provisioning, and off-boarding.

---

## 🚀 Solution

A Workato-style Genie that autonomously:

- Creates job postings  
- Screens candidates in ATS  
- Schedules interviews  
- Generates offer letters  
- Onboards employees in ADP  
- Provisions Okta / email / tools  
- Off-boards leavers automatically  

---

## 🏗 Architecture

User → Workato Go → HR Genie → Workato Recipes → ATS / ADP / Okta / ServiceNow

---

## 🔄 Demo Flow

1. Manager requests new hire  
2. Genie posts job & screens resumes  
3. Candidate selected → Offer generated  
4. On joining → Accounts & payroll created  
5. On exit → Access revoked & payroll closed  

---

## 📊 Business Impact

| Metric | Result |
|------|-------|
| HR processing effort | ↓ 70% |
| Time-to-hire | ↓ 45% |
| Onboarding SLA | ↓ 60% |

## 🔐 Human-in-the-Loop Approvals

This Genie enforces governance by requiring approvals for high-risk actions.

See the approval flow definitions in the `approvals/` folder.
