SFMC Troubleshooting Handbook
=============================

Email Studio & Deliverability
-----------------------------
- Symptom: High bounces or spam complaints.
  Resolution: Verify SAP (SPF/DKIM), DMARC alignment, warm-up IPs, list hygiene, and seed tests. Use bounce data views and ISP postmaster tools.
- Symptom: Images blocked/dark mode issues.
  Resolution: Provide alt text, avoid image-only emails, use dark-mode-safe colors, and test in major clients.

Journey Builder
---------------
- Symptom: Contacts not entering a journey.
  Resolution: Confirm entry source filters, data availability, re-entry settings, and entry schedule. Check error logs and event definitions.
- Symptom: Journey stuck or throttled.
  Resolution: Inspect wait activities, API event volume, and throttling; review contact DE indices and automation concurrency.

Automation Studio
-----------------
- Symptom: Automation fails intermittently.
  Resolution: Add error notifications, idempotent SQL, staged temp DEs, and retry patterns. Check file drops and data locks.

APIs & Integrations
-------------------
- Symptom: 401/403 on REST/SOAP.
  Resolution: Rotate client secret, validate scope, MID, package permissions, and token expiration handling.
- Symptom: Rate limit or timeouts.
  Resolution: Implement backoff retries, pagination, and job status polling.

Marketing Cloud Connect
-----------------------
- Symptom: Synchronized Data Sources stale.
  Resolution: Re-authenticate, verify user permissions and field-level security, reduce mappings, and monitor sync logs.

Data Extensions & Queries
-------------------------
- Symptom: Slow queries/timeouts.
  Resolution: Add primary keys and useful indexes, avoid SELECT *, denormalize for reads, and partition large DEs.

Compliance & Consent
--------------------
- Symptom: Sends to unsubscribed/opted-out contacts.
  Resolution: Centralize suppression checks, double-check ContactKey mapping, and enforce send classification.

References
----------
- Code samples and patterns: `https://github.com/camrobert/SalesforceMarketingCloud`
- Best practices articles: `https://www.sfmcstack.com/blog`


