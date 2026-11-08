# Radiologist can dictate codes by voice

## Purpose
As a radiologist, I can speak the short codes and have them entered as if typed.

Why: G3. Source: intent.

## Order
Order: 7 of 8
Depends on: after 2: reuses code entry (Radiologist can report multi-line pathology codes)

## Acceptance criteria
- Voice button starts and stops dictation
- Spoken codes and measurements are recognized as typed equivalents
- Recognized text is shown for correction before use
- Report is the same as for typed input

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
