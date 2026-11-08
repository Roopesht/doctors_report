# Radiologist can enter measurements and get graded wording

## Purpose
As a radiologist, I can type a code with a measurement (e.g. Li 16.2, R 8 m) and get graded size/severity wording.

Why: G1, G2. Source: doc 133 (Li ranges, kidney calculus ranges), doc 129.

## Order
Order: 4 of 8
Depends on: after 2: needs code engine (Report always covers every organ line)

## Acceptance criteria
- Liver size maps to mildly/mild to moderately/moderately/moderately to markedly/markedly using separate male and female ranges
- Measurement appears in the sentence, e.g. '(15.30 cm)'
- Kidney calculus code gives side, size 5-14.99 mm and calyx position
- Out-of-range or non-numeric input is rejected with a message

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
