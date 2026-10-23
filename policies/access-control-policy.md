# Access control policy

| | |
| --- | --- |
| ID | HG-POL-002 |
| Company | Harrowgate Digital Ltd (fictional) |
| Version | 1.0 |
| Owner | ISMS Manager |
| Date | 23 October 2026 |

## Purpose

Decide who can reach Harrowgate systems, and how that decision is reviewed.

## Rules

1. One person, one account, in the company identity provider. Shared logins are not used.
2. Production administration uses a separate admin account. Day-to-day mail is not done from that account.
3. Multi-factor authentication is required for email, the cloud tenant, the git host, the password manager, and the production console.
4. Passwords are created and stored in the company password manager. They are not reused and not sent in chat.
5. Access is requested on a ticket, approved by the asset owner, and implemented by ISMS or Engineering.
6. People tells ISMS of a leaver before the last day. Accounts are disabled that day. Shared secrets the leaver knew are rotated within five working days.
7. Every quarter, ISMS reviews production admin accounts and shared mailboxes and records who was removed.

## Portal customers

A customer firm sees only its own documents. Harrowgate staff see customer content only from an admin role that is logged. Support staff see a redacted preview unless the customer has enabled full preview.

## Related documents

HG-POL-001, asset register rows A-01, A-07, A-08, controls A.5.15 to A.5.18 and A.8.2 to A.8.5.
