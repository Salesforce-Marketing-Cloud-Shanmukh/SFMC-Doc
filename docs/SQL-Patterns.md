SQL Patterns for SFMC
=====================

Data Views
----------
- Engagement: _Open, _Click, _Sent, _Bounce, _Complaint, _Unsubscribe.
- Join keys and date filters with safe deduplication strategies.

Performance
-----------
- Use explicit column lists, avoid SELECT *.
- Primary keys and helpful indexes on DEs used frequently.
- Stage into temp DEs, then MERGE into targets for idempotency.

References
----------
- Query examples: `https://github.com/camrobert/SalesforceMarketingCloud`
- Tips and gotchas: `https://www.sfmcstack.com/blog`


