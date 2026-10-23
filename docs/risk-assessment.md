# Risk assessment

| | |
| --- | --- |
| ID | HG-ISMS-003 |
| Company | Harrowgate Digital Ltd (fictional) |
| Version | 1.0 |
| Owner | ISMS Manager |
| Date | 23 October 2026 |
| Method | ISO/IEC 27001 style risk assessment, scored by Harrowgate, not copied from the standard |

## Method

Each risk names an asset, a plausible cause, and the consequence for customers or for the company. Likelihood and impact are scored 1 to 5. The score is likelihood times impact.

| Score | Likelihood | Impact |
| --- | --- | --- |
| 1 | Not expected this year | Noticeable internally, no customer effect |
| 2 | Could happen this year | A few customers inconvenienced, or one day's staff disruption |
| 3 | Has happened in similar companies, or once here already | Customer data delayed, or a reportable near miss |
| 4 | Expected more than once a year without the control | Customer data disclosed to the wrong party, or a multi-day outage |
| 5 | Already happening or certain without the control | Wide disclosure of customer content, or a loss the company might not survive |

Appetite: scores **1–6** may be accepted by the ISMS Manager. Scores **8–12** need a treatment and an owner. Scores **15–25** are not acceptable and are escalated to the Managing Director until the residual score is 12 or below.

Treatments are **Mitigate**, **Transfer** (a contract shifts some consequence, the risk stays on the register), or **Accept**. Harrowgate does not use "avoid" in this cycle: the product cannot be offered without the production tenant.

Residual scores below already assume the controls in the [Statement of Applicability](statement-of-applicability.md) are at the status recorded there. A Partial control does not get full credit.

## Register

| ID | Risk | Assets | L | I | Score | Treatment | Residual | Owner | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| R-01 | A production admin account is phished and used to read customer documents | A-01, A-02, A-07 | 3 | 5 | 15 | Mitigate | 8 | ISMS | MFA on every admin, separate admin accounts, mail alerting on new admin grants. Residual stays at 8 because mailbox phishing of staff is still likely. |
| R-02 | A laptop with local customer files is lost or stolen | A-11, A-02 | 3 | 4 | 12 | Mitigate | 4 | ISMS | Full-disk encryption and remote wipe are required before a laptop is issued. Residual is a lost device with encryption on. |
| R-03 | The cloud tenant is misconfigured and a storage bucket is world-readable | A-02, A-23 | 3 | 5 | 15 | Mitigate | 8 | ENG | Production account is separate, public access is blocked by a tenant policy, and a monthly access review checks it. Residual stays at 8 until the review has a year of evidence. |
| R-04 | A supplier with customer content is breached | A-23, A-24, A-26 | 2 | 5 | 10 | Transfer | 8 | ISMS | Contracts name breach notice and a security contact. Harrowgate still owns the customer conversation. Top suppliers only; the long tail is an open gap, see A.5.22. |
| R-05 | Ransomware on staff endpoints reaches the file suite | A-10, A-11 | 3 | 4 | 12 | Mitigate | 6 | ISMS | Endpoint protection is on, and file-suite version history is retained. Accepted at 6. |
| R-06 | A leaver keeps access to production or email | A-07, A-01, A-10 | 3 | 4 | 12 | Mitigate | 4 | PPL | People notify ISMS on the last day. Access checklist is part of the leaver task. HR system is the trigger. |
| R-07 | A known vulnerability sits unpatched on the product or laptops | A-01, A-11 | 4 | 3 | 12 | Mitigate | 9 | ENG | Monthly scan exists. There is no agreed time limit for high findings, so residual stays at 9. Linked to Partial control A.8.8. |
| R-08 | Production data is copied into the non-production account for a test | A-05, A-02 | 3 | 4 | 12 | Mitigate | 4 | ENG | Non-production uses fabricated data. The pipeline has no path that copies the production bucket. |
| R-09 | Customer documents are unavailable for a working day | A-01, A-03 | 2 | 4 | 8 | Mitigate | 4 | ENG | Backups restore was tested in September 2026. A full ICT-readiness exercise is still planned, so A.5.30 stays Partial. |
| R-10 | One of the two IT people is unavailable during an incident | A-21, A-07 | 3 | 3 | 9 | Mitigate | 6 | MD | The Engineering Lead holds break-glass access and the incident policy names them as deputy. Accepted at 6 for a company this size. |
| R-11 | Door access at the Manchester office lets a visitor near unlocked screens | A-22, A-11 | 2 | 2 | 4 | Accept | 4 | FIN | Reception signs visitors in. Clear-desk checks are a quarterly spot check, not a guard force. |
| R-12 | Customer content is pasted into a personal mail or an unsanctioned tool | A-02, A-10 | 3 | 4 | 12 | Mitigate | 9 | ISMS | Acceptable use forbids it. Technical data-loss prevention is Planned (A.8.12), so residual stays at 9. |

## Statement of risk

The Managing Director accepts the residual scores in this register for the year to 23 October 2027. R-01, R-03, R-04, R-07, and R-12 stay above 6 and stay open. They are reviewed at the quarterly management check, and not only at the annual review. No score is at 15 or above after treatment.
