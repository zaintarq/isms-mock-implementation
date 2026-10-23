# Internal audit checklist

| | |
| --- | --- |
| ID | HG-ISMS-005 |
| Company | Harrowgate Digital Ltd (fictional) |
| Version | 1.0 |
| Auditor | Finance Lead, who does not operate the controls |
| Auditee | ISMS Manager and Engineering Lead |
| Mock audit date | 2 October 2026 |
| Report date | 9 October 2026 |

This is the checklist used for that mock audit, with the results filled in. A later audit can copy the questions and clear the result column.

Results: **Conforming**, **Minor NC** (a control or a required record is incomplete, customers are not currently exposed), **Major NC** (a required part of the system is missing or customer data is exposed), **OFI** (it conforms, and a stated improvement would make it stronger).

The audit read documents and configuration. It did not scan production. That limit is control A.8.34.

## Checklist

| ID | Ref | Question | Evidence looked for | Result |
| --- | --- | --- | --- | --- |
| C-01 | 4.1 | Are interested parties and their needs written down? | Scope, interested-party table | Conforming |
| C-02 | 4.3 | Is the scope bounded, with exclusions that make sense? | Scope in and out of scope | Conforming |
| C-03 | 5.1 | Has the Managing Director approved the security policy and the residual risks? | Signed policy, risk statement | Conforming |
| C-04 | 5.2 | Are roles named rather than left as "the team"? | Policy responsibilities, SoA owners | Conforming |
| C-05 | 5.3 | Are roles communicated to the people who hold them? | Staff handbook pointer, briefing slide | Conforming |
| C-06 | 6.1 | Is there a risk method, a register, and a risk acceptance? | HG-ISMS-003 | Conforming |
| C-07 | 6.1.3 | Does the SoA cover every Annex A control, with a reason for each exclusion? | HG-ISMS-004, 93 rows, A.7.6 and A.8.30 marked N/A | Conforming |
| C-08 | 6.2 | Are partial controls tied to an owner and a risk? | SoA partial list, R-04, R-07, R-09, R-12 | Conforming |
| C-09 | 7.2 | Can People show who completed the yearly briefing? | Attendance list | OFI |
| C-10 | 7.5 | Are ISMS documents versioned, owned, and dated? | Document headers | Conforming |
| C-11 | 8.1 | Are change, backup, and leaver procedures written and short enough to use? | Three procedures named in A.5.37 | Conforming |
| C-12 | 8.2 | Was a risk reassessment considered after the last product change that touched customer content? | Sample of three tickets | Conforming |
| C-13 | 9.1 | Is anything measured, even simply? | Quarterly admin-review record | Conforming |
| C-14 | 9.2 | Is the auditor independent of the controls they test? | Finance Lead as auditor | Conforming |
| C-15 | 9.3 | Is a management review planned, with the risk register as an input? | Quarterly check named in the risk statement | Conforming |
| C-16 | 10.1 | Is there a place to record a nonconformity and close it? | This finding log | Conforming |
| C-17 | A.5.9 | Does the asset register include every system that can see customer content? | Register versus the live supplier list | Minor NC |
| C-18 | A.5.15 | Are production admins a separate account, and was the last quarterly review done? | Review record, June 2026 | Conforming |
| C-19 | A.5.24 | Could a new starter say who to call about a lost laptop? | Incident policy, two staff asked | Conforming |
| C-20 | A.6.5 | For the last leaver, was the account disabled on the last day? | HR date versus identity-provider log | Conforming |
| C-21 | A.8.13 | Is there a restore test less than a year old? | September 2026 note | Conforming |
| C-22 | A.8.22 | Can non-production reach the production document store? | Cloud account list, no peering | Conforming |
| C-23 | A.8.31 | Was any live customer file found in the non-production account? | Bucket listing sample | Conforming |
| C-24 | A.8.34 | Did this audit avoid active testing against production? | Audit plan | Conforming |

## Finding log

### IA-2026-01 — Minor NC — asset register

**Clause.** A.5.9, checklist C-17.

**What was wrong.** On 2 October the asset register had no row for the support desk. The desk can hold snippets of customer documents, so it belongs in the inventory and on the supplier list.

**Correction.** Rows A-17 and A-26 were added on 9 October 2026. The auditor checked the rows against the live tenant name and closed the finding the same day.

**Why it was minor.** Access to the desk was already limited to the support role. The gap was the record, not an open exposure.

### IA-2026-02 — OFI — briefing completion

**Clause.** 7.2 and A.6.3, checklist C-09.

**What was seen.** The yearly briefing happened in May 2026. People could not produce a list of who was there. The control still counts as Partial.

**Suggestion.** Record completion in the HR system at the next briefing, in May 2027. No nonconformity was raised, because the briefing itself exists and the gap is already visible on the SoA.

## Auditor's conclusion

The mock ISMS hangs together: scope, assets, risks, SoA, and policies describe the same company. One record was incomplete and is now fixed. Five residual risks stay open on purpose (R-01, R-03, R-04, R-07, R-12) and were accepted by the Managing Director. This audit does not certify Harrowgate against ISO/IEC 27001. Harrowgate is fictional.
