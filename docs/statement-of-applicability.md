# Statement of Applicability

| | |
| --- | --- |
| ID | HG-ISMS-004 |
| Company | Harrowgate Digital Ltd (fictional) |
| Version | 1.0 |
| Owner | ISMS Manager |
| Date | 23 October 2026 |
| Basis | Annex A of ISO/IEC 27001:2022. Titles only. This is not the text of the standard. |

91 controls apply. 2 do not. Status is **Implemented**, **Partial**, **Planned**, or **N/A**. Partial means the control exists and a named gap is still open. Owners: MD, ISMS, ENG, PPL, FIN.

## Summary

| Status | Count |
| --- | --- |
| Implemented | 80 |
| Partial | 10 |
| Planned | 1 |
| Not applicable | 2 |

Partial: A.5.7, A.5.22, A.5.30, A.5.35, A.6.3, A.7.4, A.8.8, A.8.16, A.8.20, A.8.29. Planned: A.8.12. Not applicable: A.7.6, A.8.30.

## A.5 Organisational controls

| Control | Title | Applies | Status | Owner | Why, for Harrowgate |
| --- | --- | --- | --- | --- | --- |
| A.5.1 | Policies for information security | Yes | Implemented | MD | The policy set is approved by the MD and reviewed yearly. |
| A.5.2 | Information security roles and responsibilities | Yes | Implemented | MD | ISMS Manager owns the system. Engineering owns the product. People owns joiners and leavers. |
| A.5.3 | Segregation of duties | Yes | Implemented | ENG | The person who writes a change does not approve their own production release. |
| A.5.4 | Management responsibilities | Yes | Implemented | MD | Team leads confirm their staff have finished the annual security briefing. |
| A.5.5 | Contact with authorities | Yes | Implemented | MD | The MD is the contact for the ICO and for law enforcement. The number sits in the incident policy. |
| A.5.6 | Contact with special interest groups | Yes | Implemented | ISMS | ISMS Manager follows NCSC small-organisation guidance and the cloud supplier's security bulletins. |
| A.5.7 | Threat intelligence | Yes | Partial | ISMS | Bulletins are read ad hoc. There is no record of what was reviewed each quarter. |
| A.5.8 | Information security in project management | Yes | Implemented | ENG | A new feature that touches customer content has a short security note on the ticket before build. |
| A.5.9 | Inventory of information and other associated assets | Yes | Implemented | ISMS | The asset register is the inventory. IA-2026-01 closed the missing support-desk row. |
| A.5.10 | Acceptable use of information and other associated assets | Yes | Implemented | ISMS | Acceptable use policy, acknowledged at joining and yearly. |
| A.5.11 | Return of assets | Yes | Implemented | PPL | Leaver checklist collects the laptop, token, and shared-password handover. |
| A.5.12 | Classification of information | Yes | Implemented | ISMS | Four labels, defined on the asset register, used in policies. |
| A.5.13 | Labelling of information | Yes | Implemented | ISMS | Customer files in the portal carry the customer's own label. Internal files use the four labels in the header when they leave the file suite. |
| A.5.14 | Information transfer | Yes | Implemented | ENG | Customer content moves through the portal or company email. Personal mail and unapproved tools are forbidden. |
| A.5.15 | Access control | Yes | Implemented | ISMS | Access control policy. Default is no access until a role needs it. |
| A.5.16 | Identity management | Yes | Implemented | PPL | One identity per person in the company identity provider, opened by People, closed on the last day. |
| A.5.17 | Authentication information | Yes | Implemented | ISMS | Passwords live in the password manager. MFA is required for email, cloud, git, and production. |
| A.5.18 | Access rights | Yes | Implemented | ISMS | Quarterly review of production admins and of shared mailboxes. The review record is kept for a year. |
| A.5.19 | Information security in supplier relationships | Yes | Implemented | FIN | A supplier who can see customer content or staff data is on the asset register before the contract starts. |
| A.5.20 | Addressing information security within supplier agreements | Yes | Implemented | FIN | Those contracts include confidentiality, breach notice, and a security contact. |
| A.5.21 | Managing information security in the ICT supply chain | Yes | Implemented | ENG | Cloud and git suppliers are named. Harrowgate does not add a reseller in front of the cloud account. |
| A.5.22 | Monitoring, review and change management of supplier services | Yes | Partial | ISMS | The four high suppliers are reviewed yearly. Smaller SaaS tools are not on that cycle yet. |
| A.5.23 | Information security for use of cloud services | Yes | Implemented | ENG | Production, non-production, and logs are separate accounts. The shared responsibility note is filed with A-23. |
| A.5.24 | Information security incident management planning and preparation | Yes | Implemented | ISMS | Incident policy names roles, severity, and the first-hour actions. |
| A.5.25 | Assessment and decision on information security events | Yes | Implemented | ISMS | The ISMS Manager decides whether an event is an incident. The Engineering Lead decides if the ISMS Manager is away. |
| A.5.26 | Response to information security incidents | Yes | Implemented | ISMS | Containment is account disablement, token revoke, and isolating the affected laptop. Customer notice is the MD's decision. |
| A.5.27 | Learning from information security incidents | Yes | Implemented | ISMS | Each incident ends with a one-page note and, where needed, a risk-register change. |
| A.5.28 | Collection of evidence | Yes | Implemented | ISMS | Logs for an incident are exported to a restricted folder and left unchanged. No one edits the export. |
| A.5.29 | Information security during disruption | Yes | Implemented | MD | The incident policy still applies if the office is shut. Admin access does not depend on being in Manchester. |
| A.5.30 | ICT readiness for business continuity | Yes | Partial | ENG | A backup restore of the document store was tested in September 2026. A full exercise has not been run. |
| A.5.31 | Legal, statutory, regulatory and contractual requirements | Yes | Implemented | FIN | The register of legal duties covers UK data protection, employment records, and the security clauses in the top customer contracts. |
| A.5.32 | Intellectual property rights | Yes | Implemented | ENG | Product code is the company's. Third-party licences are recorded in the repository. |
| A.5.33 | Protection of records | Yes | Implemented | FIN | Contracts and audit records have a stated retention period in the file suite. |
| A.5.34 | Privacy and protection of PII | Yes | Implemented | MD | Customer content and staff files are Restricted. A privacy notice covers the portal and recruitment. |
| A.5.35 | Independent review of information security | Yes | Partial | MD | The October 2026 internal audit was done by the Finance Lead, who does not operate the controls. There has been no external review. |
| A.5.36 | Compliance with policies, rules and standards | Yes | Implemented | ISMS | The internal audit checklist tests the policies. Managers handle repeat breaches through the People process. |
| A.5.37 | Documented operating procedures | Yes | Implemented | ENG | Production change, backup restore, and leaver access removal are written procedures, each under two pages. |

## A.6 People controls

| Control | Title | Applies | Status | Owner | Why, for Harrowgate |
| --- | --- | --- | --- | --- | --- |
| A.6.1 | Screening | Yes | Implemented | PPL | Employees who can access customer content have a right-to-work check and one reference before access is granted. |
| A.6.2 | Terms and conditions of employment | Yes | Implemented | PPL | Contracts include confidentiality and a duty to follow the information security policy. |
| A.6.3 | Information security awareness, education and training | Yes | Partial | PPL | A yearly briefing exists. Completion is not yet tracked, so the People Lead cannot show who missed it. |
| A.6.4 | Disciplinary process | Yes | Implemented | PPL | The staff handbook already covers misconduct. A security breach uses that process. |
| A.6.5 | Responsibilities after termination or change of employment | Yes | Implemented | PPL | Access ends on the last day. Confidentiality in the contract continues. |
| A.6.6 | Confidentiality or non-disclosure agreements | Yes | Implemented | PPL | Employees sign confidentiality in the contract. Contractors sign a separate agreement before any access. |
| A.6.7 | Remote working | Yes | Implemented | ISMS | Remote work uses the company laptop, disk encryption, and MFA. Public Wi-Fi is allowed only with the laptop firewall left on. |
| A.6.8 | Information security event reporting | Yes | Implemented | ISMS | Staff report odd logins, lost devices, and wrong-recipient mail to the ISMS Manager the same day. |

## A.7 Physical controls

| Control | Title | Applies | Status | Owner | Why, for Harrowgate |
| --- | --- | --- | --- | --- | --- |
| A.7.1 | Physical security perimeters | Yes | Implemented | FIN | The leased suite has a locked door off a reception. There is no other site. |
| A.7.2 | Physical entry | Yes | Implemented | FIN | Staff use landlord tokens. Visitors are signed in. Tokens are disabled on the leaver checklist. |
| A.7.3 | Securing offices, rooms and facilities | Yes | Implemented | FIN | The suite is locked when the last person leaves. A key-holder list has three names. |
| A.7.4 | Physical security monitoring | Yes | Partial | FIN | The landlord operates shared-area cameras. Harrowgate has no written way to request footage after an incident. |
| A.7.5 | Protecting against physical and environmental threats | Yes | Implemented | FIN | The office is a serviced building with the landlord's fire detection. Laptops are the production path, so a closed office does not stop the service. |
| A.7.6 | Working in secure areas | No | N/A | FIN | There is no secure area. No room has rules beyond the normal office. |
| A.7.7 | Clear desk and clear screen | Yes | Implemented | ISMS | Screens lock at five minutes. Customer content is not left on paper overnight. |
| A.7.8 | Equipment siting and protection | Yes | Implemented | ISMS | Laptops are issued with a lock cable for the office. Servers are not kept on site. |
| A.7.9 | Security of assets off-premises | Yes | Implemented | ISMS | Laptops leaving the office stay encrypted and are not left in a car overnight. |
| A.7.10 | Storage media | Yes | Implemented | ISMS | USB storage is blocked on company laptops. Removable media is not used for customer content. |
| A.7.11 | Supporting utilities | Yes | Implemented | FIN | Power and connectivity in the office are the landlord's. The service itself runs in the cloud, so an office power cut is not a customer outage. |
| A.7.12 | Cabling security | Yes | Implemented | FIN | Office network cabling is in the landlord's floor boxes. Harrowgate does not run its own comms room. |
| A.7.13 | Equipment maintenance | Yes | Implemented | ISMS | Laptops are replaced on a three-year cycle or when they can no longer take security updates. |
| A.7.14 | Secure disposal or re-use of equipment | Yes | Implemented | ISMS | Disks are wiped or destroyed before a laptop is sold or returned. A one-line record is kept. |

## A.8 Technological controls

| Control | Title | Applies | Status | Owner | Why, for Harrowgate |
| --- | --- | --- | --- | --- | --- |
| A.8.1 | User endpoint devices | Yes | Implemented | ISMS | Company laptops only, with disk encryption, screen lock, and endpoint protection. |
| A.8.2 | Privileged access rights | Yes | Implemented | ISMS | Production admin is a separate account, held by two people, reviewed quarterly. |
| A.8.3 | Information access restriction | Yes | Implemented | ENG | Portal users see only their firm's documents. Staff admin access is logged. |
| A.8.4 | Access to source code | Yes | Implemented | ENG | The repository is private. Write access is the engineering team. Production secrets are not stored in git. |
| A.8.5 | Secure authentication | Yes | Implemented | ISMS | MFA on email, cloud, git, VPN-equivalent identity, and the production console. |
| A.8.6 | Capacity management | Yes | Implemented | ENG | Cloud capacity alerts are set on the production account. A review happens when an alert fires, and monthly otherwise. |
| A.8.7 | Protection against malware | Yes | Implemented | ISMS | Endpoint protection is on every laptop and alerts the ISMS Manager. |
| A.8.8 | Management of technical vulnerabilities | Yes | Partial | ENG | A monthly vulnerability scan covers the product and laptop OS versions. High findings have no agreed fix time. |
| A.8.9 | Configuration management | Yes | Implemented | ENG | Laptop build is a standard image. Production baseline is the infrastructure code in the repository. |
| A.8.10 | Information deletion | Yes | Implemented | ENG | Customer content is deleted when the contract ends, after the retention window in the contract. Backups age out on the same window. |
| A.8.11 | Data masking | Yes | Implemented | ENG | Support staff see document names and a redacted preview, not the full file, unless the customer turns full preview on. |
| A.8.12 | Data leakage prevention | Yes | Planned | ISMS | No DLP product is in place. The acceptable use rule is the only control. Target date 31 March 2027. |
| A.8.13 | Information backup | Yes | Implemented | ENG | Document store and database are backed up daily. Restore was tested in September 2026. |
| A.8.14 | Redundancy of information processing facilities | Yes | Implemented | ENG | Production runs across two availability zones in the UK region. There is no second vendor. |
| A.8.15 | Logging | Yes | Implemented | ENG | Admin actions and portal access are logged to the logging account. Logs are kept for one year. |
| A.8.16 | Monitoring activities | Yes | Partial | ISMS | Alerts exist for new admin grants and for endpoint malware. There is no out-of-hours rota, which matches a 50-person company and is accepted under R-10. |
| A.8.17 | Clock synchronization | Yes | Implemented | ENG | Cloud and laptops use the provider time service so log times can be compared. |
| A.8.18 | Use of privileged utility programs | Yes | Implemented | ENG | Break-glass cloud roles are the only utilities that can bypass normal admin. Their use pages the ISMS Manager. |
| A.8.19 | Installation of software on operational systems | Yes | Implemented | ISMS | Staff cannot install unsigned software. The laptop image allows a short approved list. |
| A.8.20 | Networks security | Yes | Partial | ENG | Production network rules default to deny. The office network is the landlord's shared Wi-Fi, which Harrowgate does not control, so office traffic is treated as untrusted. |
| A.8.21 | Security of network services | Yes | Implemented | ENG | The portal is HTTPS only. Admin interfaces are not published to the whole internet. |
| A.8.22 | Segregation of networks | Yes | Implemented | ENG | Production, non-production, and logging are separate cloud accounts with no peering from non-production into production data. |
| A.8.23 | Web filtering | Yes | Implemented | ISMS | Laptop DNS blocks known malware domains. A full web-category filter is not used. |
| A.8.24 | Use of cryptography | Yes | Implemented | ENG | Customer content is encrypted in transit and at rest with the cloud provider's keys, stored in the cloud secret service. |
| A.8.25 | Secure development life cycle | Yes | Implemented | ENG | Design note, peer review, and a test pass are required before production. |
| A.8.26 | Application security requirements | Yes | Implemented | ENG | New portal features state who can see the data and how long it is kept, on the ticket. |
| A.8.27 | Secure system architecture and engineering principles | Yes | Implemented | ENG | The written principle is least privilege, separate accounts, and no customer data in non-production. |
| A.8.28 | Secure coding | Yes | Implemented | ENG | Peer review includes a short secure-coding checklist. Dependencies are pinned. |
| A.8.29 | Security testing in development and acceptance | Yes | Partial | ENG | Peer review and unit tests gate a release. There is no regular external test. |
| A.8.30 | Outsourced development | No | N/A | ENG | Product code is written by employees and by individuals onboarded as contractors. There is no outsourced development supplier. |
| A.8.31 | Separation of development, test and production environments | Yes | Implemented | ENG | Separate cloud accounts. Production data is not copied across. |
| A.8.32 | Change management | Yes | Implemented | ENG | A production change needs a ticket, a second reviewer, and a same-day rollback note. |
| A.8.33 | Test information | Yes | Implemented | ENG | Tests use fabricated firms and documents. A customer file in a test ticket is treated as an incident. |
| A.8.34 | Protection of information systems during audit testing | Yes | Implemented | ISMS | This internal audit reads records and configuration. It does not run scans against production. Any later technical test needs the Engineering Lead's written window. |
