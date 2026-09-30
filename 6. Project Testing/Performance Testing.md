# Performance Testing

## Project Title
Auto Ticket Classification using Flow Designer

## Objective

The objective of testing is to verify that the ServiceNow Flow Designer correctly classifies school IT support tickets and performs the required actions.

## Testing Approach

The project was tested by creating Incident WorkFlow records with different issue descriptions.

The Flow Designer checks the Short Description and automatically assigns the appropriate Category and Subcategory.

## Test Cases

| Test Case | Short Description | Expected Category | Expected Subcategory |
|---|---|---|---|
| 1 | WiFi not working in library | Network | Wi-Fi |
| 2 | Projector not turning on | Hardware | Projector |
| 3 | Forgot password | Access | Forgot Password |
| 4 | Slow Computer | Performance | Slow Computer |

## Email Notification Testing

After ticket classification, an email notification is sent to the Caller.

The email subject used in the project is:

**Your Request for the issue has been submitted.**

The email can be verified from:

**All → Emails → System Logs → Emails**

The required email can be searched using its subject and previewed to verify the notification.

## Validation

The following points were validated:

- Incident WorkFlow record is created successfully.
- Flow is triggered when the Category is empty.
- Short Description is checked for the supported issue keywords.
- Correct Category is assigned.
- Correct Subcategory is assigned.
- Email notification is sent to the Caller.
- Different issue types are handled through separate Flow Designer branches.

## Result

The testing confirms that the implemented Flow Designer performs the required automatic ticket classification and email notification functions for the supported test cases.

## Conclusion

The project was tested using different school IT support scenarios. The classification and notification functions were validated according to the project requirements.
