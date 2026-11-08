# Radiologist can start a report for a male or female patient

## Purpose
As a radiologist, I can enter patient details and choose male or female so the right template is used.

Why: G4 (templates by sex). Source: docs 127, 128.

## Order
Order: 1 of 8
Depends on: none

## Acceptance criteria
- Header fields (name, age, referred by, date, UHID, Sr. No) can be entered
- Sex selection (Mr./Mrs.) is required before codes are accepted
- Male selects the prostate template, female the uterus/ovaries template
- Date defaults to today

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
