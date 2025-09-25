Detailed Data Model
===================

Data Extensions
---------------
- Contacts (PK: ContactKey): EmailAddress, Locale, PreferencesRef, CreatedDate.
- Consent (PK: ContactKey, Channel): Status, Source, Timestamp, Proof.
- Transactions: OrderId, ContactKey, ItemsJSON, Revenue, Timestamp.
- Events: EventId, ContactKey, Type, AttributesJSON, Timestamp.

Indexes & Retention
-------------------
- Primary keys and secondary indexes on ContactKey and event timestamps.
- Retention: rolling windows with anonymization for expired records.

Mappings
--------
- Salesforce SObjects to SFMC DEs via MC Connect and custom APIs.
- Field-level security and transformation rules documented here.


