# Project Executable Files

## Project Title
Auto Ticket Classification using Flow Designer

## Project Platform

The project is implemented using the ServiceNow platform and Flow Designer.

## Executable / Project Components

The project contains the following main components:

1. Incident WorkFlow custom table
2. Caller field
3. Category field
4. Subcategory field
5. Short Description field
6. Description field
7. State field
8. Assigned Group field
9. Assigned To field
10. Auto Classification Flow
11. Email Notification
12. Project Update Set

## Flow Designer

Flow Name:

**Auto Classify School IT Tickets**

The flow is triggered when a new Incident WorkFlow record is created and the Category is empty.

The flow checks the Short Description and assigns the appropriate Category and Subcategory.

## Classification

- Wi-Fi issue → Network → Wi-Fi
- Projector issue → Hardware → Projector
- Forgot Password → Access → Forgot Password
- Slow Computer → Performance → Slow Computer

## Deployment File

The ServiceNow project configuration can be transferred using the exported:

**Project_Update_Set.xml**

## Project Execution

The project is executed within the ServiceNow instance. After creating a ticket, the Flow Designer automatically processes the ticket and sends an email notification to the Caller.
