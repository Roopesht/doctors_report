# Radiologist can type codes and get the normal-findings report

## Purpose
As a radiologist, I can type short codes (e.g. Li, P, S, NF, NL, U) and get the matching normal-finding sentences in the fixed template order.

Why: G2, G4. Source: doc 133 abbreviation table, docs 127/128.

## Order
Order: 2 of 8
Depends on: after 1: needs sex/template (Radiologist can start a report for a male or female patient)

## Acceptance criteria
- Each known code yields its exact sentence from doc 133
- Output order follows the male/female template regardless of typing order
- Male report matches doc 127 wording; female matches doc 128
- Unknown code is flagged, not dropped silently
- Normal report ends with 'IMPRESSION: USG whole abdomen reveals no obvious abnormality.'

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
