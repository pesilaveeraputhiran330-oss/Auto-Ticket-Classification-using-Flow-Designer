# Solution Requirements

## Functional Requirements

1. The system should automatically classify school IT helpdesk tickets.
2. The system should identify the issue from the Short Description.
3. The system should automatically assign the appropriate Category.
4. The system should automatically assign the dependent Subcategory.
5. The system should send a confirmation email to the Caller.
6. The system should store ticket information in the Incident WorkFlow table.

## Categories

- Network
- Hardware
- Access
- Performance

## Subcategories

- Wi-Fi
- Projector
- Forgot Password
- Slow Computer

## Category-Subcategory Dependency

| Category | Subcategory |
|---|---|
| Network | Wi-Fi |
| Hardware | Projector |
| Access | Forgot Password |
| Performance | Slow Computer |

## Data Requirements

The system should maintain fields such as:

- Number
- Caller
- Category
- Subcategory
- Short Description
- Description
- State
- Assigned Group
- Assigned To

## Maintainability and Scalability

The Flow Designer automation should be maintainable and scalable for future ticket classification requirements.
