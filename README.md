# ISMS mock implementation

Research pack for a **fictional** 50-person company, Harrowgate Digital Ltd. It is a lightweight information security management system: scope, asset register, risk assessment, Statement of Applicability, a short policy set, and an internal audit checklist.

Harrowgate Digital does not exist. Nothing here is a certificate, a client deliverable, or the text of ISO/IEC 27001. Control names are used so the Statement of Applicability can be read against the 2022 edition. The implementation notes are original and describe only this made-up company.

## The company

Harrowgate Digital builds **Client Ledger**, a hosted portal where professional-services firms exchange documents with their own clients. About 50 people work from one Manchester office and from home in the UK. Two of them cover IT and the ISMS between them. The interesting data is customer contact data and client documents, stored in a UK-region cloud tenant. Card payments are taken by a hosted checkout, so cardholder data stays outside the company.

## Document map

| ID | Document | What it decides |
| --- | --- | --- |
| HG-ISMS-001 | [Scope](docs/scope.md) | What the ISMS covers, and what it leaves out |
| HG-ISMS-002 | [Asset register](docs/asset-register.md) | The information, systems, and suppliers that matter |
| HG-ISMS-003 | [Risk assessment](docs/risk-assessment.md) | How risks are scored, and the current register |
| HG-ISMS-004 | [Statement of Applicability](docs/statement-of-applicability.md) | Which Annex A controls apply, and how far they are in place |
| HG-POL-001 | [Information security policy](policies/information-security-policy.md) | The policy the Managing Director signs |
| HG-POL-002 | [Access control policy](policies/access-control-policy.md) | Accounts, MFA, and access reviews |
| HG-POL-003 | [Acceptable use policy](policies/acceptable-use-policy.md) | What staff may do with customer content |
| HG-POL-004 | [Incident management policy](policies/incident-management-policy.md) | How an event is reported and closed |
| HG-POL-005 | [Backup and recovery policy](policies/backup-and-recovery-policy.md) | Daily backups and the yearly restore test |
| HG-POL-006 | [Supplier security policy](policies/supplier-security-policy.md) | Contracts before a supplier sees data |
| HG-ISMS-005 | [Internal audit checklist](docs/internal-audit-checklist.md) | How an internal audit would test this pack |

Owners used throughout: Managing Director (MD), ISMS Manager (ISMS), Engineering Lead (ENG), People Lead (PPL), Finance Lead (FIN).

## How the pieces fit

The scope names Client Ledger, the company laptops, and the suppliers who can see customer data. The asset register lists those things and gives each one an owner and a classification. The risk register scores what could go wrong with them. The Statement of Applicability says which controls were chosen because of those risks, including two controls that do not apply. The policies are the short set a 50-person company can actually maintain. The checklist is what the internal auditor walked through on 2 October 2026 in this mock, including one minor finding that was closed a week later.

## Status

| | |
| --- | --- |
| Pack version | 1.0 |
| Date | 23 October 2026 |
| Next review | 23 October 2027 |
| Classification | Internal to the fictional company. Published here only as research. |
