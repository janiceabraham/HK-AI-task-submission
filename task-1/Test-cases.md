## Test Cases

The following five synthetic test cases evaluate the proposed SIS announcement notification workflow.

| Test Case | Input | Expected Result | Recovery / Control |
|---|---|---|---|
| TC01: Normal Announcement | An authorised publisher submits a complete announcement. | The announcement is published through the authorised process, and a notification is generated with a link to SIS. | Retry failed delivery and use an available fallback channel. |
| TC02: Missing Information | An announcement is missing a required title or deadline. | The system flags missing information before publication or notification, where validation is supported. | Return it to the authorised publisher for correction. |
| TC03: Duplicate Announcement | A new announcement has details similar to an existing notice. | The system flags a possible duplicate for review. | An authorised person determines whether it is a duplicate, correction, or new announcement. |
| TC04: Unauthorised Request | A user without publication permission attempts to publish or modify an announcement. | The request is rejected by the applicable access controls. | Refer the request to an authorised person and record the event if logging is supported. |
| TC05: Notification Failure | An announcement is published, but its email notification fails. | The failure is identified, and the system attempts a retry or available in-portal fallback. | Escalate persistent failures to technical support. The original SIS announcement remains available. |

### Evaluation Criteria

- Valid announcements trigger notifications.
- Missing required information is flagged.
- Possible duplicates are identified for human review.
- Unauthorised publication attempts are blocked.
- Notification failures trigger recovery procedures.
- Original announcements remain accessible through SIS.
- The notification process follows the applicable approval procedures.

**Testing Status:** These are proposed test cases with expected results. They have not been executed on the live SIS portal and require validation in an approved test environment.
