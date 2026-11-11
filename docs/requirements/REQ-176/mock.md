# Mock: Radiologist can start a report for a male or female patient

Sketch only of what the documents describe.

```
+------------------------------------------+
| New report                               |
|------------------------------------------|
| Name        [______________]  Age [___]  |
| Sex         ( ) Mr. (Male)  ( ) Mrs. (Female) |
| Referred by [______________]             |
| Date        [today's date  ]             |
| UHID No     [______________]             |
| Sr. No      [______________]  (manual)   |
|                                          |
| [Start report]                           |
+------------------------------------------+

Flow:
  Fill header -> select Mr./Mrs. -> template loads
     Mr.  -> prostate template
     Mrs. -> uterus/ovaries template
  No sex selected -> codes are not accepted
```
