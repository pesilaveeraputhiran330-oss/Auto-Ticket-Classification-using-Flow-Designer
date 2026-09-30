# Auto-Ticket-Classification-using-Flow-Designer
## Project Overview

Auto Ticket Classification using Flow Designer is a ServiceNow automation project designed to automatically classify school IT support tickets.

The system identifies the type of issue from the ticket's Short Description and automatically assigns the appropriate Category and Subcategory.

## Problem Statement

School IT helpdesk receives different types of IT support incidents such as:

- Wi-Fi problems
- Projector problems
- Forgot password issues
- Slow computer problems

Manual classification can take time and may result in inconsistent classification.

## Proposed Solution

The project uses ServiceNow Flow Designer to automatically classify newly created Incident WorkFlow records.

The flow checks the Short Description and assigns the corresponding Category and Subcategory.

## Classification

| Issue | Category | Subcategory |
|---|---|---|
| Wi-Fi | Network | Wi-Fi |
| Projector | Hardware | Projector |
| Forgot Password | Access | Forgot Password |
| Slow Computer | Performance | Slow Computer |

## Main Features

- Incident WorkFlow custom table
- Auto Number generation
- Caller information
- Category management
- Subcategory management
- Category-Subcategory dependency
- Automatic ticket classification
- Automatic Category assignment
- Automatic Subcategory assignment
- Email notification
- Structured ticket storage
- Update Set deployment

## Technology Used

- ServiceNow
- Flow Designer
- Custom Table
- Update Sets
- XML Export

## Working Flow

```text
Create IT Ticket
       ↓
Incident WorkFlow
       ↓
Record Created Trigger
       ↓
Check Short Description
       ↓
Identify IT Issue
       ↓
Assign Category
       ↓
Assign Subcategory
       ↓
Send Email to Caller
