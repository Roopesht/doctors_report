# Radiologist can review, edit and export the report

## Purpose
As a radiologist, I can review and edit the generated report and export it in the layout of docs 127/128.

Why: G4. Source: docs 127, 128.

## Order
Order: 8 of 8
Depends on: after 5: needs complete report (Radiologist can dictate codes by voice)

## Acceptance criteria
- Preview shows header, findings, impression and signature block
- Text can be edited before export
- Export keeps the doc 127/128 layout
- Signature block is Dr. Pankaj Singhal, MD Radio Diagnosis, HMC – HN004918 as in the sample

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
