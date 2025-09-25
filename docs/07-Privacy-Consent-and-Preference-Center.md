Privacy, Consent, and Preference Center
======================================

Compliance Framework
--------------------
- GDPR, CCPA, CAN-SPAM, CASL: lawful basis, notice, choice, and control.
- Data retention and minimization for marketing data extensions.

Consent Data Model
------------------
- Centralized consent object keyed by ContactKey with channel-level flags.
- Double opt-in flows with time-stamped audit trail.
- Integration with Salesforce Individual object where applicable.

Preference Center Architecture
------------------------------
- Public CloudPages for subscription management and profile updates.
- Authentication, CSRF protection, and rate limiting for API endpoints.
- Eventing to update journeys and suppressions in near real-time.


