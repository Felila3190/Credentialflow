CredentialFlow — Workflow Specification

Version: 1.0
Year: 2026

Save Time. Stop the Chasing. One Easy Go-To.

⸻

1. Purpose

This document defines the core workflow that CredentialFlow will use to manage workforce credentials.

The workflow connects worker actions, system status changes, notifications and management decisions into one structured process.

⸻

2. Core CredentialFlow

WORKER
   ↓
UPLOAD
   ↓
SUBMIT
   ↓
VERIFY / REVIEW
   ↓
STATUS
   ↓
TRACK
   ↓
REMIND
   ↓
ACTION REQUIRED
   ↓
EXPLAIN / REQUEST
   ↓
MANAGEMENT REVIEW
   ↓
APPROVE / DECLINE
   ↓
STATUS UPDATED

⸻

3. Worker Workflow

Step 1 — Access

The worker signs into CredentialFlow using their authorised account.

The system identifies the worker and displays the credentials associated with their profile.

⸻

Step 2 — View Credentials

The worker can view their credential list.

Each credential should display information such as:

* Credential name
* Status
* Issue date
* Expiry date
* Verification status
* Required action

⸻

Step 3 — Select Credential

The worker selects a credential requiring submission or updating.

CredentialFlow displays the relevant information required for that credential.

⸻

Step 4 — Upload

The worker uploads the relevant credential document.

The system should confirm that the document has been received.

The uploaded document should be associated with the appropriate credential record.

⸻

Step 5 — Enter Credential Details

The worker enters applicable information, including:

* Credential type
* Credential/reference number where applicable
* Issue date
* Expiry date
* Issuing organisation where applicable

The system should validate required fields before allowing submission.

⸻

Step 6 — Submit

The worker submits the credential.

The credential status changes to:

SUBMITTED

Where verification is required, the next status may become:

VERIFICATION PENDING

⸻

4. Verification Workflow

Where an authorised verification process is available:

SUBMITTED
    ↓
VERIFICATION PENDING
    ↓
VERIFICATION
    ↓
VERIFIED

If verification cannot be completed, the system should allow an appropriate outcome or management review rather than incorrectly marking the credential as verified.

CredentialFlow must not claim that a credential has been independently verified when no authorised verification has occurred.

⸻

5. Credential Tracking

CredentialFlow continuously tracks credential status against applicable dates and requirements.

The system should identify credentials that are:

* Current
* Expiring soon
* Expired
* Missing
* Verification pending
* Awaiting action

⸻

6. Expiry Workflow

A credential approaching expiry should trigger the applicable reminder process.

Example:

CURRENT
   ↓
EXPIRING SOON
   ↓
EXPIRY DATE
   ↓
EXPIRED

Reminder timing should be configurable by the organisation.

Example reminder schedule:

* 30 days before expiry
* 14 days before expiry
* 7 days before expiry
* On expiry
* Follow-up after expiry where required

⸻

7. Overdue Workflow

When a credential becomes overdue:

EXPIRED
   ↓
ACTION REQUIRED
   ↓
WORKER RESPONSE

The worker may be asked to:

* Upload the renewed credential
* Provide an explanation
* Enter an expected document date
* Request an extension where appropriate

⸻

8. Explanation Workflow

The worker may submit an explanation for an overdue credential.

The explanation should be linked to the relevant credential record.

The system should record:

* Explanation
* Date submitted
* Worker
* Credential
* Expected document date where provided

⸻

9. Extension Request Workflow

Where organisational policy permits an extension request:

OVERDUE
   ↓
EXPLANATION
   ↓
EXTENSION REQUEST
   ↓
MANAGEMENT REVIEW

The request should contain the information required for management to make an informed decision.

⸻

10. Management Review

An authorised management user receives the request for review.

The management interface should provide:

* Worker
* Credential
* Current status
* Expiry date
* Explanation
* Expected document date
* Supporting information where applicable
* Request date

Management can then choose:

APPROVE

or

DECLINE

⸻

11. Approval Workflow

If approved:

EXTENSION REQUESTED
        ↓
EXTENSION APPROVED
        ↓
NEW ACTION / REVIEW DATE

The system should record the decision and the authorised decision-maker.

Approval should not automatically mean that the underlying credential has been verified or renewed.

⸻

12. Decline Workflow

If declined:

EXTENSION REQUESTED
        ↓
EXTENSION DECLINED
        ↓
ACTION REQUIRED

The worker should be informed of the decision and any required next action, subject to organisational policy.

⸻

13. Management Dashboard

The management dashboard should prioritise action.

A management user should be able to quickly identify:

Current

Credentials currently meeting requirements.

Expiring Soon

Credentials approaching expiry.

Expired

Credentials that have passed their expiry date.

Missing

Required credentials that have not been submitted.

Verification Pending

Credentials awaiting an applicable verification process.

Extension Requests

Requests requiring management attention.

⸻

14. Notifications

Notifications should be triggered by defined workflow events.

Potential events include:

* Credential approaching expiry
* Credential expired
* Credential submitted
* Verification required
* Verification completed
* Extension request submitted
* Extension approved
* Extension declined

Notification delivery may eventually support multiple channels.

⸻

15. Audit Trail

Important actions should create an audit event.

Example:

03 Sep 2026
Credential uploaded
Worker
04 Sep 2026
Credential submitted
Worker
04 Sep 2026
Verification pending
System
10 Sep 2026
Extension requested
Worker
11 Sep 2026
Extension approved
Manager

The audit trail should provide a chronological record of relevant actions.

⸻

16. Exception Handling

CredentialFlow should recognise that not every credential situation can follow the standard pathway.

Possible exceptions include:

* Document unavailable
* Credential awaiting renewal
* Verification unavailable
* Incorrect document submitted
* Expiry information unclear
* Extension required
* Management review required

Exceptions should be visible rather than hidden.

⸻

17. Status Principle

Every credential should have a clear current status.

The system should avoid ambiguous states wherever possible.

The primary objective is that a user can answer:

What is the status?

and:

What happens next?

without manually searching through emails, spreadsheets or folders.

⸻

18. Permission Principle

CredentialFlow should apply role-based permissions.

Workers should access their own permitted credential information.

Management should access information necessary for their authorised responsibilities.

Administrative functions should be restricted to authorised users.

⸻

19. Future Integration Points

The workflow should be designed so authorised integrations can be added later.

Potential integration areas may include:

* Authorised credential verification
* Training systems
* Workforce management platforms
* HR systems
* Notification services
* Identity/authentication services

Integrations should only be implemented where appropriate, authorised and technically feasible.

⸻

20. Core Product Principle

CredentialFlow should turn credential administration from:

SCATTERED INFORMATION

into:

ONE CLEAR WORKFLOW

And from:

MANUAL CHASING

into:

STRUCTURED ACTIONS

The intended experience is simple:

Upload → Track → Know → Act

⸻

CredentialFlow

Save Time. Stop the Chasing. One Easy Go-To.

Founded & created by Felila Aiga
2026
