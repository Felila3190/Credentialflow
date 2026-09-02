CredentialFlow — Screen Specification

Version: 1.0
Year: 2026

Save Time. Stop the Chasing. One Easy Go-To.

⸻

1. Purpose

This document defines the primary screens and navigation structure for the CredentialFlow MVP.

The interface should be simple, clear and action-focused.

The system should allow users to quickly understand:

What is my status?

and:

What do I need to do next?

⸻

2. User Roles

CredentialFlow MVP will have two primary user experiences:

Worker

Manages their own credentials and responds to required actions.

Management

Monitors workforce credentials and manages review and decision workflows.

⸻

3. Worker Navigation

The worker interface should provide access to:

Dashboard
│
├── My Credentials
│
├── Notifications
│
├── Requests
│
└── Profile

⸻

4. Worker Dashboard

The worker dashboard should provide an immediate overview.

Suggested sections

Credential Summary

* Current
* Expiring soon
* Expired
* Missing
* Verification pending

Action Required

A prominent section showing credentials requiring the worker’s attention.

Upcoming Expiries

Credentials approaching their expiry dates.

Recent Activity

Recent credential submissions, verification updates and requests.

⸻

5. My Credentials

This screen displays the worker’s credentials.

Each credential should show:

* Credential name
* Status
* Expiry date
* Verification status
* Required action

Example:

First Aid Certificate
Status: VERIFIED
Expires: 01 June 2027
NDIS Worker Screening
Status: EXPIRING SOON
Expires: 18 October 2026
Action: Renewal required

⸻

6. Credential Detail

Selecting a credential opens the credential detail screen.

The screen may display:

* Credential name
* Credential number where applicable
* Issue date
* Expiry date
* Issuing organisation
* Current status
* Verification status
* Uploaded document
* Required action
* Relevant history

The worker should be able to update or replace information where permitted.

⸻

7. Upload Credential

The upload screen should provide a simple process.

Step 1

Select credential type.

Step 2

Upload document.

Step 3

Enter required details.

Step 4

Review information.

Step 5

Submit.

The system should confirm successful submission.

⸻

8. Overdue Credential

When a credential becomes overdue, the worker should receive a clear action screen.

Example:

Credential Expired
Your First Aid Certificate has expired.
Expiry date:
01 June 2026
What would you like to do?
[ Upload Renewed Credential ]
[ Explain Delay ]
[ Request Extension ]

Available options should depend on organisational policy and workflow configuration.

⸻

9. Explanation Screen

The worker can provide an explanation for an overdue credential.

Fields may include:

Explanation

Text field.

Expected Document Date

Date field.

Supporting Information

Optional field where appropriate.

The worker then selects:

Submit Explanation

or

Request Extension

⸻

10. Extension Request Screen

The extension request should display:

* Credential
* Expiry date
* Explanation
* Expected document date
* Supporting information where permitted

The worker should be required to confirm the information before submission.

After submission:

Status: EXTENSION REQUESTED

⸻

11. Request Status

Workers should be able to view submitted requests.

Example:

First Aid Certificate
Extension Request
Status:
PENDING MANAGEMENT REVIEW
Submitted:
03 September 2026
Expected document:
15 September 2026

Possible outcomes:

* Pending
* Approved
* Declined

⸻

12. Notifications

The worker notification area should display important actions.

Examples:

Credential Expiring

Your credential expires in 14 days.

Credential Expired

Your credential requires attention.

Verification Update

Your credential has been verified.

Extension Decision

Your extension request has been approved.

Notifications should direct the worker to the relevant action.

⸻

13. Management Navigation

Management navigation should provide:

Management Dashboard
│
├── Workforce
│
├── Credentials
│
├── Verification
│
├── Extension Requests
│
├── Notifications
│
└── Audit History

⸻

14. Management Dashboard

The management dashboard should prioritise information requiring action.

Summary

Display counts for:

* Current
* Expiring soon
* Expired
* Missing
* Verification pending
* Extension requests

Priority Actions

Display items requiring immediate or timely attention.

Recent Activity

Display recent credential submissions, verification events and management decisions.

⸻

15. Workforce View

Management should be able to view authorised workforce members and their credential status.

Example:

Worker             Current   Expiring   Expired   Action
---------------------------------------------------------
Worker 001            5         1          0        Review
Worker 002            4         0          1        Action
Worker 003            6         0          0        None

The actual information displayed should be governed by user permissions.

⸻

16. Credential Review

Management can select a credential requiring review.

The review screen may display:

* Worker
* Credential type
* Document
* Issue date
* Expiry date
* Submission date
* Verification status
* Current status
* Relevant history

Available actions depend on the workflow.

⸻

17. Verification Review

Where verification is required, management or an authorised verification process should be able to identify:

Verification Pending

The screen should provide the information necessary to complete or monitor the applicable verification process.

Possible outcomes may include:

* Verified
* Unable to verify
* Further information required
* Management review required

CredentialFlow should not mark a credential as verified without an appropriate verification outcome.

⸻

18. Extension Request Review

Management should have a dedicated review screen.

Example:

Extension Request
Worker:
Worker 001
Credential:
First Aid Certificate
Expiry:
01 June 2026
Explanation:
Renewal appointment scheduled.
Expected document:
15 September 2026
Decision:
[ APPROVE ]
[ DECLINE ]

The system should require an authorised management user to make the decision.

⸻

19. Decision Confirmation

Before completing a management decision, the system should clearly identify the action.

Example:

Approve Extension?
Credential:
First Aid Certificate
Worker:
Worker 001
New review date:
15 September 2026
[ Confirm Approval ]
[ Cancel ]

A similar confirmation should be used when declining a request.

⸻

20. Audit History

Management should be able to view relevant historical actions.

Example:

03 Sep 2026 — Credential uploaded
03 Sep 2026 — Credential submitted
03 Sep 2026 — Verification pending
10 Sep 2026 — Extension requested
11 Sep 2026 — Extension approved

Audit history should identify the relevant user/system action and timestamp.

⸻

21. Design Principles

CredentialFlow screens should follow these principles:

Simple

Avoid unnecessary complexity.

Clear

Status and required actions should be immediately understandable.

Action-focused

Users should know what to do next.

Accessible

The interface should be designed for a broad range of users.

Consistent

Status terminology and navigation should remain consistent throughout the platform.

Secure

Sensitive information should only be displayed to authorised users.

⸻

22. MVP Screen List

Worker

1. Login
2. Dashboard
3. My Credentials
4. Credential Detail
5. Upload Credential
6. Overdue Credential
7. Explanation
8. Extension Request
9. Request Status
10. Notifications
11. Profile

Management

1. Login
2. Management Dashboard
3. Workforce
4. Credential Review
5. Verification Review
6. Extension Requests
7. Decision Confirmation
8. Notifications
9. Audit History

⸻

23. Core Interface Principle

CredentialFlow should make the answer visible:

What is the status?

and:

What happens next?

The interface should reduce the need for users to search through documents, emails or spreadsheets to determine the next action.

⸻

CredentialFlow

Save Time. Stop the Chasing. One Easy Go-To.

Founded & created by Felila Aiga
2026
