# Proposed Solution

## Solution Overview

The project uses ServiceNow Flow Designer to automatically classify school IT helpdesk tickets based on the Short Description.

## How the Solution Works

1. A new Incident WorkFlow record is created.
2. The Flow Designer is triggered when Category is empty.
3. The flow checks the Short Description.
4. The flow identifies the issue using keyword conditions.
5. The corresponding Category and Subcategory are updated.
6. A confirmation email is sent to the Caller.

## Classification Logic

| Condition in Short Description | Category | Subcategory |
|---|---|---|
| Wi-Fi / Network | Network | Wi-Fi |
| Projector | Hardware | Projector |
| Forgot Password | Access | Forgot Password |
| Slow Computer | Performance | Slow Computer |

## Main Components

- Incident WorkFlow custom table
- Record Created trigger
- If / Else If classification branches
- Update Record actions
- Send Email action

## Expected Benefits

- Automatic ticket classification
- Consistent Category and Subcategory assignment
- Automatic caller notification
- Structured ticket processing
- Maintainable automation

## Solution Flow

User submits IT issue  
↓  
Incident WorkFlow record is created  
↓  
Flow Designer is triggered  
↓  
Short Description is checked  
↓  
Issue is identified  
↓  
Category and Subcategory are updated  
↓  
Confirmation email is sent to Caller
