# Technology Stack

## Platform

### ServiceNow
ServiceNow is used as the platform for creating and managing the IT helpdesk ticket automation.

## Automation Tool

### Flow Designer
ServiceNow Flow Designer is used to automatically classify the IT helpdesk tickets based on the Short Description.

## Database / Data Storage

### ServiceNow Custom Table
A custom table named **Incident WorkFlow** is used to store the IT helpdesk ticket information.

## Main Components

- Incident WorkFlow table
- Custom fields
- Category and Subcategory
- Reference fields
- Flow Designer
- Record Created trigger
- Update Record action
- Send Email action
- Update Set

## Automation Logic

The Flow Designer checks the Short Description and updates the appropriate Category and Subcategory.

## Deployment

The project configuration is maintained using a **Project Update Set**, which can be completed and exported as XML.
