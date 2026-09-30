# Data Flow Diagram

## Input

The user provides IT helpdesk ticket details:

- Caller
- Short Description
- Description

## Process

1. A new Incident WorkFlow record is created.
2. Flow Designer is triggered when the Category is empty.
3. The flow checks the Short Description.
4. The issue is identified based on keywords.
5. The appropriate Category and Subcategory are updated.
6. A confirmation email is sent to the Caller.

## Classification Flow

Short Description
        ↓
Flow Designer
        ↓
Check Issue Keyword
        ↓
Category + Subcategory
        ↓
Update Incident WorkFlow Record
        ↓
Send Confirmation Email to Caller

## Output

The system produces:

- Classified Category
- Appropriate Subcategory
- Updated Incident WorkFlow record
- Confirmation email to Caller

## Classification Examples

Wi-Fi / Network issue
→ Network → Wi-Fi

Projector issue
→ Hardware → Projector

Forgot Password
→ Access → Forgot Password

Slow Computer
→ Performance → Slow Computer
