# Coding & Solution

## Overview

The Auto Ticket Classification project is implemented as a no-code solution using ServiceNow Flow Designer.

Instead of traditional programming code, the solution uses table configuration, fields, choice values, dependencies and Flow Designer actions.

## 1. Custom Table

A custom table named **Incident WorkFlow** is created to store IT helpdesk ticket records.

### Main Fields

| Field | Type |
|---|---|
| Number | Auto Number |
| Caller | Reference – sys_user |
| Category | Choice |
| Subcategory | Choice |
| Short Description | String |
| Description | String |
| State | Choice |
| Assigned Group | Reference – sys_user_group |
| Assigned To | Reference – sys_user |

## 2. Category Configuration

The Category field contains:

- Network
- Hardware
- Access
- Performance

## 3. Subcategory Configuration

The Subcategory field contains:

- Wi-Fi
- Projector
- Forgot Password
- Slow Computer

## 4. Category Dependency

The Subcategory field is configured as dependent on Category.

| Subcategory | Category |
|---|---|
| Wi-Fi | Network |
| Projector | Hardware |
| Forgot Password | Access |
| Slow Computer | Performance |

## 5. Flow Designer

### Flow Name

**Auto Classify School IT Tickets**

### Trigger

- Trigger: Record Created
- Table: Incident WorkFlow
- Condition: Category is Empty

## 6. Classification Logic

### Wi-Fi / Network

If the Short Description contains Wi-Fi or Network:

```text
Category = Network
Subcategory = Wi-Fi
