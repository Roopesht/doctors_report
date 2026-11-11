# Radiologist can start a report for a male or female patient

## Purpose
As a radiologist, I can enter patient details and choose male or female so the right report template is used.

Why: G4 (templates by sex). Source: docs 127, 128.

## Order
Order: 1 of 8
Depends on: none

## Behaviour
1. The radiologist opens a new report and sees the header form.
2. The radiologist enters the header fields: name, age, referred by, date, UHID No and Sr. No.
3. Date is pre-filled with today's date; the radiologist may change it.
4. Sr. No is typed in by the radiologist. It is never auto-generated.
5. The radiologist selects the sex: Mr. (male) or Mrs. (female). Nothing is selected by default.
6. Once the sex is selected, the matching template is loaded:
   - Male: prostate template
   - Female: uterus/ovaries template
7. Until the sex is selected, codes are not accepted for this report.

## Acceptance criteria
- Header fields (name, age, referred by, date, UHID No, Sr. No) can be entered.
- Sr. No is entered manually by the radiologist (not auto-generated).
- Sex selection (Mr./Mrs.) is required before codes are accepted.
- Male selects the prostate template, female the uterus/ovaries template.
- Date defaults to today.

## Questions and answers
No questions were raised for this requirement, so there are no answers to apply. The open questions in the earlier draft (code syntax, full code list, default text per missing organ, male/female liver ranges, voice engine, export format) concern code entry, report content and export. They are outside the scope of this requirement and belong to the later requirements that cover those areas.

## Out of scope
- Entering codes and measurements (later requirements).
- Report content defaults, voice input and export.

## Source documents
- docs/project/intent.md
- docs/project/source/ (docs 127, 128, 129, 133)
