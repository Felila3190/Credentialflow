CredentialFlow — MVP Product Requirements

Version: 1.0
Year: 2026
Founder & Creator: Felila Aiga

Save Time. Stop the Chasing. One Easy Go-To.

⸻

1. Product Overview

CredentialFlow is a workforce credential management platform designed to simplify the process of collecting, monitoring, reviewing and maintaining worker credentials.

The MVP will provide a structured workflow allowing workers and management to manage credential information from submission through to review, renewal and exception handling.

Core workflow

Upload → Verify → Track → Remind → Explain / Request → Review → Decide

The MVP is intended to demonstrate that credential administration can be made clearer, more structured and less dependent on repetitive manual follow-up.

⸻

2. MVP Objective

The primary objective of the MVP is to demonstrate a functioning credential-management workflow that can:

* Centralise credential information
* Provide clear credential status
* Identify credentials requiring attention
* Reduce repetitive manual follow-up
* Support renewal reminders
* Allow workers to explain overdue credentials
* Allow workers to request extensions where appropriate
* Allow authorised management users to review and decide requests
* Maintain an auditable history of important actions

The MVP should prioritise clarity, usability, security and measurable outcomes over feature volume.

⸻

3. Primary Users

3.1 Worker

Workers use CredentialFlow to manage their own credential information.

A worker should be able to:

* Sign in securely
* View required credentials
* Select a credential type
* Upload a credential document
* Enter relevant credential information
* Enter issue and expiry dates
* View credential status
* Receive renewal reminders
* Respond to overdue credentials
* Provide an explanation
* Enter an expected document date
* Submit an extension request
* View the outcome of an extension request

⸻

3.2 Management

Authorised management users use CredentialFlow to monitor workforce credential compliance.

Management should be able to:

* View workforce credential status
* Identify missing credentials
* Identify expiring credentials
* Identify expired credentials
* Identify verification-pending credentials
* Review submitted credential information
* Review overdue explanations
* Review extension requests
* Approve or decline extension requests
* View outstanding actions
* Access an audit history

⸻

4. Credential Status

CredentialFlow will use clear status categories to communicate the current state of each credential.

MISSING

A required credential has not yet been submitted.

SUBMITTED

A worker has submitted a credential for processing or review.

VERIFICATION PENDING

The credential requires verification through an appropriate authorised process.

VERIFIED

The credential has passed the applicable verification process.

EXPIRING SOON

The credential is approaching its expiry date.

EXPIRED

The credential has passed its expiry date.

EXTENSION REQUESTED

The worker has submitted an explanation and requested an extension.

EXTENSION APPROVED

An authorised management user has approved the extension.

EXTENSION DECLINED

An authorised management user has declined the extension.

⸻

5. Worker Workflow

The core worker journey should follow:

Login

↓

My Credentials

↓

Select Credential

↓

Upload Document

↓

Enter Credential Details

↓

Submit

↓

Verification / Review

↓

Status Updated

↓

Reminder / Action Required

Overdue workflow

If a credential becomes overdue:

Credential becomes overdue

↓

Worker receives notification

↓

Worker provides explanation

↓

Worker enters expected document date

↓

Worker submits extension request

↓

Management review

↓

Approve / Decline

↓

Credential status updated

⸻

6. Management Workflow

The management journey should provide a clear overview of workforce credential requirements.

The management dashboard should allow authorised users to identify:

* Current credentials
* Expiring credentials
* Expired credentials
* Missing credentials
* Verification-pending credentials
* Extension requests
* Outstanding actions

The dashboard should prioritise items requiring attention.

⸻

7. Notifications & Reminders

CredentialFlow should support automated reminders to reduce repetitive manual follow-up.

A future production configuration may include reminders such as:

* 30 days before expiry
* 14 days before expiry
* 7 days before expiry
* On expiry
* After expiry where action remains outstanding

Reminder timing should be configurable rather than permanently hard-coded.

Management notifications should also be triggered when appropriate, including:

* New credential submission
* Verification requiring review
* Extension request submitted
* Extension request approved
* Extension request declined
* Credential remaining overdue

⸻

8. Extension Request Workflow

CredentialFlow should provide a structured alternative to informal overdue follow-up.

A worker may provide:

* Explanation for the delay
* Expected document date
* Supporting information where required
* Extension request

The request should then be presented to an authorised management user.

Management should be able to:

Approve

or

Decline

The system should record:

* Request date
* Worker
* Credential
* Explanation
* Expected document date
* Decision
* Decision date
* Decision-maker
* Relevant notes

⸻

9. Verification

CredentialFlow should support verification workflows where an appropriate authorised verification source or integration exists.

The MVP should clearly distinguish between:

Document submission

and

Credential verification

CredentialFlow must not represent a credential as independently verified unless an authorised verification process has actually occurred.

The initial prototype may therefore use a simulated or demonstration verification state.

Production verification integrations would be developed separately and only where technically, legally and organisationally appropriate.

⸻

10. Audit Trail

Important actions should be recorded to provide accountability and traceability.

Examples include:

* Credential uploaded
* Credential updated
* Credential submitted
* Verification initiated
* Verification completed
* Credential status changed
* Reminder issued
* Explanation submitted
* Extension requested
* Extension approved
* Extension declined

Each relevant event should record information such as:

* Action
* Date and time
* User
* Credential
* Result or status

⸻

11. Access & Permissions

CredentialFlow should use role-based access.

Worker

Access should be limited to the worker’s own credential information and permitted actions.

Management

Access should be limited according to organisational role and authorisation.

Administrator

Administrative access should be restricted to authorised system functions.

The principle of least-privilege access should guide the platform design.

⸻

12. Security & Privacy Principles

CredentialFlow is intended to handle potentially sensitive workforce information.

The production system should therefore be designed with:

* Secure authentication
* Role-based permissions
* Secure document storage
* Encryption where appropriate
* Access controls
* Audit logging
* Secure data transmission
* Appropriate data retention policies
* Secure deletion processes
* Privacy-by-design principles

The MVP prototype should not use real worker credentials or unnecessary personal information.

⸻

13. MVP Scope

Included

* Worker credential management
* Credential upload
* Credential details
* Expiry tracking
* Credential status
* Management dashboard
* Reminder workflow
* Overdue workflow
* Extension requests
* Management decisions
* Audit history
* Role-based access concept

Not initially included

* Payroll
* Rostering
* Recruitment
* Performance management
* Full HR management
* Every possible credential type
* Every government verification database
* Large-scale enterprise integrations
* Native mobile applications
* Advanced artificial intelligence features

These may be considered during later development stages.

⸻

14. Success Criteria

The MVP should demonstrate that a worker can:

1. Access CredentialFlow
2. Select a required credential
3. Upload a document
4. Enter credential information
5. Submit the credential
6. View its status
7. Receive or trigger an appropriate reminder
8. Respond to an overdue credential
9. Submit an extension request
10. Receive a management decision

The MVP should also demonstrate that authorised management can:

1. View workforce credential status
2. Identify items requiring attention
3. Review submitted information
4. Review extension requests
5. Approve or decline requests
6. View relevant action history

⸻

15. Pilot Measurement

CredentialFlow’s proposed target of reducing credential administration time by up to 50% is a development target, not a proven result.

A controlled pilot should establish a baseline before measuring improvement.

Potential measures include:

* Time spent following up credentials
* Number of manual reminders
* Time spent reviewing credential status
* Processing time for overdue requests
* Number of outstanding actions
* Worker completion rates
* Management user experience
* Worker user experience

Measurement approach

Measure → Test → Improve → Validate

The purpose is to replace assumptions with measurable evidence.

⸻

16. MVP Principle

CredentialFlow should not attempt to become an entire workforce-management platform.

The MVP should focus on solving one clear problem:

How can organisations manage workforce credentials with less chasing and clearer visibility?

The product should remain simple enough for workers to understand and powerful enough for management to act.

⸻

17. Future Development

Following successful MVP testing, CredentialFlow may be expanded to include:

* Additional credential types
* Authorised verification integrations
* Advanced reporting
* Configurable organisational workflows
* Additional notification channels
* Accessibility enhancements
* Mobile applications
* Organisation-level analytics
* Additional workforce environments
* Expanded integrations

Future features should be prioritised according to pilot evidence, user needs, technical feasibility and security requirements.

⸻

18. Product Vision

CredentialFlow aims to move workforce credential management from:

“Where is it?”

to:

“What is the status, and what happens next?”

The long-term vision is to create a practical, secure and measurable workflow that reduces administrative chasing and gives workforce teams more time for the people and services they support.

⸻

CredentialFlow

Save Time. Stop the Chasing. One Easy Go-To.

Founded & created by Felila Aiga
2026
