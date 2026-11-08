# Radiologist can report multi-line pathology codes

## Purpose
As a radiologist, I can use codes for gall bladder, pancreas, uterus/ovary, free fluid and bladder-filling findings, with blanks I fill in.

Why: G2. Source: doc 133 (Gall bladder, PC, Uterus, UB2/UB3, free fluid, RPOC, etc.).

## Order
Order: 6 of 8
Depends on: after 5: uses impression logic (Impression matches the findings)

## Acceptance criteria
- Each code yields its finding and its impression where the doc gives one
- '....' placeholders prompt for a value before output
- Sex-specific codes are refused for the wrong sex
- UB3 adds 'TVS may be advised' impression

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
