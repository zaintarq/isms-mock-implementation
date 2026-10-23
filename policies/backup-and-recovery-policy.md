# Backup and recovery policy

| | |
| --- | --- |
| ID | HG-POL-005 |
| Company | Harrowgate Digital Ltd (fictional) |
| Version | 1.0 |
| Owner | Engineering Lead |
| Date | 23 October 2026 |

## Purpose

Be able to get customer documents back, and to know that the copies work.

## Rules

1. The production database and the document store are backed up at least daily.
2. Backups stay in the UK, in a second region, in the same cloud provider. They are encrypted with the same key-management approach as production.
3. Backup admin is a production admin account. It is not granted to the whole engineering team.
4. Backups are kept for the retention period in the customer contract, then they age out with production data.
5. A restore of the document store is tested at least once a year. The September 2026 test is the current record. The result is a short note: what was restored, how long it took, and what failed.
6. A full exercise that includes telling customers about a delay is still planned. Until that happens, control A.5.30 stays Partial and risk R-09 stays open at residual 4.

## If production is unavailable

Engineering leads the restore. The ISMS Manager handles the incident record. The Managing Director decides what customers are told if the outage will pass one working day.

## Related documents

Asset rows A-01, A-02, A-03, risk R-09, controls A.5.30 and A.8.13.
