# Sample Project Documentation

## Project Title

Auto Ticket Classification using Flow Designer

## Problem Statement

School IT helpdesk receives different types of IT support incidents such as Wi-Fi problems, projector problems, password issues and slow computers.

Manual classification of these tickets can take time and may result in inconsistent classification.

## Proposed Solution

A ServiceNow Flow Designer automation is used to automatically classify IT support tickets based on the Short Description.

The system assigns the appropriate Category and Subcategory and sends an email notification to the Caller.

## Categories

| Category | Subcategory |
|---|---|
| Network | Wi-Fi |
| Hardware | Projector |
| Access | Forgot Password |
| Performance | Slow Computer |

## Main Components

- Incident WorkFlow custom table
- Category and Subcategory fields
- Category-Subcategory dependency
- Flow Designer
- Record Created trigger
- Conditional branches
- Update Record action
- Send Email action
- Update Set

## Working Flow

```text
Create IT Ticket
       ↓
Incident WorkFlow
       ↓
Flow Designer Trigger
       ↓
Check Short Description
       ↓
Identify Issue
       ↓
Assign Category
       ↓
Assign Subcategory
       ↓
Send Email to Caller
