# Solution Architecture

## Architecture Overview

The solution uses ServiceNow Flow Designer to automate the classification of school IT helpdesk tickets.

## Architecture Flow

```text
School IT Helpdesk User
          ↓
   Incident WorkFlow
          ↓
    Record Created
       Trigger
          ↓
    Flow Designer
          ↓
  Check Short Description
          ↓
     ┌────┴────┐
     ↓         ↓
Identify     Identify
 Wi-Fi       Projector
     ↓         ↓
 Network     Hardware
  + Wi-Fi    + Projector
     
     ↓
Identify Forgot Password
     ↓
Access + Forgot Password

     ↓
Identify Slow Computer
     ↓
Performance + Slow Computer
          ↓
    Update Ticket
          ↓
   Send Email to Caller
