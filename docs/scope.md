# Scope statement

| | |
| --- | --- |
| ID | HG-ISMS-001 |
| Company | Harrowgate Digital Ltd (fictional) |
| Version | 1.0 |
| Approved by | Managing Director |
| Date | 23 October 2026 |
| Next review | 23 October 2027 |

## Organisation

Harrowgate Digital Ltd is a 50-person product company. It designs, operates, and supports Client Ledger, a web portal in which professional-services firms store and share documents with their clients. Staff work from a single leased office in Manchester and from homes in the UK. There is no second office, no data centre, and no in-house development team outside the company.

Interested parties that affect the ISMS:

| Party | What they need from Harrowgate |
| --- | --- |
| Customers (the firms) | Their clients' documents stay confidential and available |
| Customers' clients | Personal data in those documents is handled lawfully |
| Staff | A clear, small set of rules and working laptops |
| Managing Director | No surprise that would threaten the customer contracts |
| Cloud, email, payroll, and support-desk suppliers | A defined security contact and a contract that matches access |
| UK ICO, as regulator for personal data | A lawful basis and a way to answer a request |

## In scope

The ISMS covers:

- Client Ledger production and the UK-region cloud tenant it runs in, including identity, storage, logs, and backups of customer content
- The source code repository, build pipeline, and the separate non-production environment
- Company-issued laptops and phones used for work, including home use
- Corporate email, files, the password manager, CRM, finance system, payroll system, and support desk
- The people who administer those systems, and the joiners, movers, and leavers process
- Suppliers who host the systems above or who can access customer content or staff personal data
- The Manchester office for the hours Harrowgate staff are in it, limited to access control of the company area and the handling of paper records

## Out of scope

- The landlord's building systems, lifts, and shared-area CCTV, except where Harrowgate relies on the landlord for office access control. That reliance is a supplier matter, not a Harrowgate-operated control room.
- Cardholder data. Checkout is hosted by the payment provider. Harrowgate does not receive or store card numbers.
- Personal equipment belonging to a customer's own clients.
- Products and networks of customers, beyond the tenant the customer is given inside Client Ledger.
- Development done by anyone who is not an employee or a contracted individual onboarded through the People process. Harrowgate does not outsource product development.

## Boundaries

A change is inside the ISMS when it can read, change, or delete customer content, staff personal data, or the keys and admin roles that protect them. A marketing page with no customer data can sit outside the engineering change path, and it is still subject to the acceptable use and incident rules if it is on a company account.

The scope is reviewed yearly, and whenever a new supplier can see customer content or a new office opens.
