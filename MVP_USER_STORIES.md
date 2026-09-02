CredentialFlow — MVP User Stories

Version: 1.0
Year: 2026

Save Time. Stop the Chasing. One Easy Go-To.

⸻

1. Purpose

User stories describe what CredentialFlow users need to accomplish and why.

They will be used to guide MVP development and testing.

⸻

2. Worker User Stories

WF-01 — Access Credentials

As a worker,
I want to access my credential records,
so that I can understand what credentials I currently have and what requires attention.

Acceptance Criteria

* Worker can access their credential list.
* Only authorised credentials are displayed.
* Each credential has a clear status.
* Expiry information is visible where applicable.

⸻

WF-02 — Upload Credential

As a worker,
I want to upload a credential document,
so that my credential information can be submitted for review.

Acceptance Criteria

* Worker can select a credential type.
* Worker can upload a supported document.
* Worker can enter required credential information.
* Worker can submit the credential.
* System confirms successful submission.

⸻

WF-03 — View Credential Status

As a worker,
I want to see the current status of my credential,
so that I know whether I need to take action.

Acceptance Criteria

The system displays an understandable status such as:

* Current
* Expiring Soon
* Expired
* Missing
* Verification Pending
* Extension Requested
* Verified

⸻

WF-04 — Receive Renewal Reminder

As a worker,
I want to receive reminders before my credential expires,
so that I have time to renew it.

Acceptance Criteria

* Reminder timing can be configured.
* Reminder identifies the relevant credential.
* Reminder identifies the expiry date.
* Reminder provides an appropriate next action.

⸻

WF-05 — Respond to Overdue Credential

As a worker,
I want to respond when a credential becomes overdue,
so that management can understand the situation.

Acceptance Criteria

Worker can:

* View the overdue credential.
* Provide an explanation.
* Enter an expected document date.
* Submit the information.

⸻

WF-06 — Request Extension

As a worker,
I want to request an extension where permitted,
so that management can review my circumstances.

Acceptance Criteria

* Worker can initiate an extension request.
* Worker provides an explanation.
* Worker can provide an expected document date.
* Request is submitted to authorised management.
* Request status is visible to the worker.

⸻

WF-07 — View Request Outcome

As a worker,
I want to see the outcome of my extension request,
so that I know what action is required next.

Acceptance Criteria

Request can display:

* Pending
* Approved
* Declined

The relevant decision date should be recorded.

⸻

3. Management User Stories

MG-01 — View Workforce Status

As a management user,
I want to see workforce credential status,
so that I can quickly identify items requiring attention.

Acceptance Criteria

Management can view authorised workforce credential information.

The dashboard identifies:

* Current
* Expiring
* Expired
* Missing
* Verification Pending
* Extension Requests

⸻

MG-02 — Review Credential

As a management user,
I want to review submitted credentials,
so that I can determine whether further action is required.

Acceptance Criteria

Management can view permitted credential information including:

* Worker
* Credential type
* Document
* Issue date
* Expiry date
* Status
* Verification status

⸻

MG-03 — Identify Expiring Credentials

As a management user,
I want to identify credentials approaching expiry,
so that renewal can occur before the credential expires.

Acceptance Criteria

* Expiring credentials are clearly identified.
* Expiry dates are visible.
* Relevant action is displayed.

⸻

MG-04 — Identify Overdue Credentials

As a management user,
I want to identify overdue credentials,
so that outstanding compliance actions are visible.

Acceptance Criteria

* Expired credentials are identifiable.
* Relevant worker is displayed where authorised.
* Required action is visible.
* Management can access the relevant credential record.

⸻

MG-05 — Review Extension Request

As a management user,
I want to review an extension request,
so that I can make an informed decision.

Acceptance Criteria

Management can view:

* Worker
* Credential
* Expiry date
* Explanation
* Expected document date
* Supporting information where applicable
* Request date

⸻

MG-06 — Approve Extension

As an authorised management user,
I want to approve an extension request,
so that the credential workflow can reflect my decision.

Acceptance Criteria

* Management can select approve.
* System requests confirmation.
* Approval is recorded.
* Decision-maker is recorded.
* Decision date is recorded.
* Worker can see the outcome.
* Audit event is created.

⸻

MG-07 — Decline Extension

As an authorised management user,
I want to decline an extension request,
so that the worker knows further action is required.

Acceptance Criteria

* Management can select decline.
* System requests confirmation.
* Decision is recorded.
* Decision-maker is recorded.
* Decision date is recorded.
* Worker can see the outcome.
* Audit event is created.

⸻

4. Verification User Stories

VR-01 — Verification Pending

As a management user,
I want to identify credentials awaiting verification,
so that they do not remain unnoticed.

Acceptance Criteria

* Verification-pending credentials are clearly identified.
* Relevant credential information is available.
* Verification status can be updated through an authorised process.

⸻

VR-02 — Verification Outcome

As an authorised verifier or system process,
I want to record a verification outcome,
so that CredentialFlow accurately reflects the credential’s verification state.

Acceptance Criteria

Possible outcomes may include:

* Verified
* Unable to verify
* Further information required
* Management review required

The system must not automatically mark a credential as verified merely because a document has been uploaded.

⸻

5. Notification User Stories

NT-01 — Worker Notification

As a worker,
I want to receive relevant credential notifications,
so that I know when action is required.

⸻

NT-02 — Management Notification

As a management user,
I want to receive notifications when management action is required,
so that requests and exceptions are not overlooked.

Examples include:

* Extension request
* Verification review
* Overdue credential
* Important credential status change

⸻

6. Audit User Stories

AU-01 — Record Actions

As an organisation,
I want important CredentialFlow actions recorded,
so that there is an accountable history of activity.

Acceptance Criteria

Important events should record:

* Event
* Date and time
* Relevant user
* Relevant credential
* Outcome where applicable

⸻

7. Security User Stories

SE-01 — Role-Based Access

As an organisation,
I want users to have access appropriate to their role,
so that credential information is not unnecessarily exposed.

Acceptance Criteria

* Worker access is restricted.
* Management access is authorised.
* Administrative functions are restricted.
* Sensitive information is protected.

⸻

8. MVP Priority

User stories should be developed in the following priority order.

Priority 1 — Core

* WF-01 Access Credentials
* WF-02 Upload Credential
* WF-03 View Credential Status
* MG-01 View Workforce Status
* MG-02 Review Credential

Priority 2 — Workflow

* WF-04 Receive Renewal Reminder
* WF-05 Respond to Overdue Credential
* WF-06 Request Extension
* MG-05 Review Extension Request
* MG-06 Approve Extension
* MG-07 Decline Extension

Priority 3 — Supporting Systems

* Verification
* Notifications
* Audit history
* Role-based permissions

⸻

9. MVP Definition of Done

The CredentialFlow MVP can be considered functionally demonstrated when:

Worker can

* Access credentials
* Upload a credential
* View its status
* Receive an expiry/action notification
* Respond to an overdue credential
* Submit an extension request
* View the decision

Management can

* View workforce status
* Identify credentials requiring attention
* Review credentials
* Review extension requests
* Approve or decline requests
* View relevant activity history

System can

* Maintain credential status
* Trigger appropriate workflow events
* Record important actions
* Apply role-based access principles

⸻

10. Product Principle

Every feature should ultimately support the central purpose of CredentialFlow:

Save Time. Stop the Chasing. One Easy Go-To.

If a feature does not make credential management clearer, easier, safer or more measurable, it should be questioned before being added to the MVP.

⸻

CredentialFlow

Save Time. Stop the Chasing. One Easy Go-To.

Founded & created by Felila Aiga
2026
