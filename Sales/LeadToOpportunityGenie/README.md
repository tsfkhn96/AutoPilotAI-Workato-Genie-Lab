# Lead-to-Opportunity Sales Genie

An autonomous Sales AI agent that converts chat messages into Salesforce leads
and opportunities automatically.

---

## 🧩 Problem

Sales reps waste time manually entering leads and updating CRM systems.

---

## 🚀 Solution

A Workato-style Genie that:

- Accepts natural language lead requests
- Creates Salesforce Lead
- Checks duplicates
- Converts to Opportunity
- Assigns owner automatically
- Notifies sales team in Slack

---

## 🏗 Architecture

Sales Rep → Workato Go → Sales Genie → Workato Recipes → Salesforce / Slack

---

## 🔄 Demo Flow

User types:

> "Create lead for John from Tesla, email john@tesla.com, deal value $50k"

Genie actions:

1. Extract lead info  
2. Create Salesforce Lead  
3. Check for duplicates  
4. Convert to Opportunity  
5. Assign owner  
6. Send Slack confirmation  

---

## 📊 Business Impact

| Metric | Result |
|------|-------|
| CRM data entry time | ↓ 70% |
| Lead conversion speed | ↑ 3× |
| Data quality | ↑ significantly |
