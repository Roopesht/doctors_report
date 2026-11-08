# Impression matches the findings

## Purpose
As a radiologist, I can get an impression generated from the findings, with no contradicting impressions.

Why: G1. Source: doc 133 (IMPRESSION lines, 'Remove all impressions of Hepatomegaly/Splenomegaly/Hepatosplenomegaly'), doc 129.

## Order
Order: 5 of 8
Depends on: after 4: needs graded findings (Radiologist can enter measurements and get graded wording)

## Acceptance criteria
- Each finding with an impression adds it (e.g. Mild hepatomegaly)
- Severity in impression equals severity from the measurement
- Remove-impression rule drops listed impressions
- Normal impression is not shown when any abnormal impression exists
- Multiple impressions are listed in order

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
