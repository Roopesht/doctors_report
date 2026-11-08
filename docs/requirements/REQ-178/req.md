# Report always covers every organ line

## Purpose
As a radiologist, I can rely on every organ line being present, with a default line when I typed no code for it.

Why: G5. Source: intent, docs 127/128, doc 133 (e.g. PD 'not clearly visualized').

## Order
Order: 3 of 8
Depends on: after 2: extends code-to-report (Radiologist can type codes and get the normal-findings report)

## Acceptance criteria
- Every organ line of the sex template appears in the report
- Organ without code gets a default (normal or not visualized) per rule
- Radiologist is told which organs were defaulted
- Codes for not-visualized organs (PD, UNV) override the default

## Source documents
- docs/project/intent.md
- docs/project/source/ (docs 127, 128, 129, 133)

## Open questions
- Exact code syntax (spaces, case, how measurements and sides are typed) is not defined in the documents.
- Full list of codes: several rows of doc 133 are unclear or lack a code (e.g. 'Ecfwfc', 'LMOT', 'HSOCS').
- Default text per missing organ (normal vs not visualized) is not defined; Not goals are unconfirmed.
- Female liver ranges and male ranges appear mixed in doc 133 (Li lines); confirm which set is male.
- Voice engine and language/accent are not defined.
- Export format (docx, PDF, print) is not defined; doc 127/128 header/signature variability is unknown.
