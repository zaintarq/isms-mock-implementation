# Asset register

| | |
| --- | --- |
| ID | HG-ISMS-002 |
| Company | Harrowgate Digital Ltd (fictional) |
| Version | 1.0 |
| Owner | ISMS Manager |
| Date | 23 October 2026 |

Classification is **Public**, **Internal**, **Confidential**, or **Restricted**. Restricted means customer content or secrets that would let someone read it. Criticality is how badly a day of loss would hurt customers: High, Medium, or Low.

The support-desk row was missing at the mock internal audit on 2 October 2026. It was added on 9 October, which closed finding IA-2026-01. See the [checklist](internal-audit-checklist.md).

| ID | Asset | Type | Owner | Where it lives | Classification | Personal data | Criticality |
| --- | --- | --- | --- | --- | --- | --- | --- |
| A-01 | Client Ledger production | Application | ENG | UK-region cloud tenant | Restricted | Yes, customer content | High |
| A-02 | Customer document store | Data | ENG | Same tenant, separate bucket | Restricted | Yes | High |
| A-03 | Production backups | Data | ENG | Same cloud, second region in the UK | Restricted | Yes | High |
| A-04 | Production audit logs | Data | ISMS | Cloud logging account | Confidential | Limited identifiers | High |
| A-05 | Non-production environment | Application | ENG | Separate cloud account, no live customer data | Internal | No | Medium |
| A-06 | Source code and build pipeline | Application | ENG | Company git host and CI | Confidential | No | High |
| A-07 | Company identity provider | Service | ISMS | Cloud identity tenant | Restricted | Staff accounts | High |
| A-08 | Admin and signing credentials | Secret | ISMS | Password manager and cloud secret store | Restricted | No | High |
| A-09 | TLS certificates | Secret | ENG | Cloud certificate service | Confidential | No | Medium |
| A-10 | Company email and files | Service | ISMS | Collaboration suite | Confidential | Yes, staff and customer mail | High |
| A-11 | Staff laptops | Device | ISMS | Issued to each employee, disk encrypted | Confidential | Yes, local copies | High |
| A-12 | Staff phones used for MFA | Device | ISMS | Personal or company phones enrolled for MFA | Internal | No customer content expected | Medium |
| A-13 | Password manager | Service | ISMS | Vendor SaaS | Restricted | Shared secrets | High |
| A-14 | CRM | Service | FIN | Vendor SaaS | Confidential | Customer contacts | Medium |
| A-15 | Finance system | Service | FIN | Vendor SaaS | Confidential | Invoices, not card numbers | Medium |
| A-16 | Payroll and HR files | Service | PPL | Vendor SaaS | Restricted | Staff personal data | High |
| A-17 | Support desk | Service | ENG | Vendor SaaS | Confidential | Customer tickets, sometimes document snippets | High |
| A-18 | Corporate website | Service | ENG | Static host, no customer store | Public | No | Low |
| A-19 | Customer contracts | Record | FIN | Contract folder in the file suite | Confidential | Business contacts | Medium |
| A-20 | Employee contracts and screening notes | Record | PPL | HR system | Restricted | Yes | Medium |
| A-21 | ISMS document set | Record | ISMS | This repository's fictional original lives in the company file suite | Internal | No | Medium |
| A-22 | Office door access | Physical | FIN | Landlord tokens for the Manchester suite | Internal | No | Low |
| A-23 | Cloud infrastructure supplier | Supplier | ENG | UK regions used by A-01 to A-04 | Restricted | Processes customer content | High |
| A-24 | Email and file supplier | Supplier | ISMS | Hosts A-10 | Confidential | Processes staff and customer mail | High |
| A-25 | Payroll supplier | Supplier | PPL | Hosts A-16 | Restricted | Processes staff data | High |
| A-26 | Support-desk supplier | Supplier | ENG | Hosts A-17 | Confidential | Processes ticket content | High |
| A-27 | Payment checkout supplier | Supplier | FIN | Hosted checkout, no card data returned | Confidential | Payment status only | Medium |

Paper on desks is not a separate asset. The acceptable use policy says customer content is not printed unless the Engineering Lead agrees, and printed copies are shredded the same day.
