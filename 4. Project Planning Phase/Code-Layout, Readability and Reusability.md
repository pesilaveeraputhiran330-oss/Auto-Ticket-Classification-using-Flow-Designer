# Code Layout, Readability and Reusability

## Overview

This project is developed using ServiceNow Flow Designer as a no-code automation solution.

The implementation is organized into a custom table, structured fields, dependent choices, Flow Designer conditions, record update actions and email notification.

## Project Layout

```text
ServiceNow Application
│
├── Incident WorkFlow Table
│   ├── Number
│   ├── Caller
│   ├── Category
│   ├── Subcategory
│   ├── Short Description
│   ├── Description
│   ├── State
│   ├── Assigned Group
│   └── Assigned To
│
├── Category & Subcategory Dependency
│
└── Flow Designer
    ├── Record Created Trigger
    ├── Wi-Fi Classification
    ├── Projector Classification
    ├── Password Classification
    ├── Slow Computer Classification
    ├── Update Record
    └── Send Email
