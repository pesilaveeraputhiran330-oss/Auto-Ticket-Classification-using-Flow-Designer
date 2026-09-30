# Customer Journey Map

## User
School IT Helpdesk User

## 1. Identify the Issue
The user experiences an IT issue such as:
- Wi-Fi / Network issue
- Projector issue
- Forgot Password
- Slow Computer

## 2. Submit the Request
The user provides the Caller details and enters the issue in the Short Description and Description fields.

## 3. Ticket Creation
A new record is created in the Incident WorkFlow table in ServiceNow.

## 4. Automatic Classification
The Flow Designer checks the Short Description and identifies the type of IT issue.

## 5. Category and Subcategory Assignment
The system automatically assigns the appropriate Category and dependent Subcategory.

## 6. Email Notification
A confirmation email is sent to the Caller after the request is processed.

## 7. Expected Outcome
The ticket is classified correctly and the user receives confirmation of the submitted request.

## Journey Summary

User identifies issue
        ↓
Submits IT request
        ↓
Incident WorkFlow record created
        ↓
Flow Designer checks Short Description
        ↓
Category and Subcategory assigned
        ↓
Confirmation email sent to Caller
