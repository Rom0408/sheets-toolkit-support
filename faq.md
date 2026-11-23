# FAQ (support page + canned replies for Phase 3 auto-support)

**Does it see or store my data?** No. It runs inside your sheet only; nothing is sent anywhere.
**Why does =GREG2HEB show an empty cell?** Input must be a real date, not text. Use Clean selection first, or =DATEVALUE().
**HEB2GREG returns empty.** Format: `day month year`, e.g. `ט״ו בניסן תשפ״ד` or `15 ניסן 5784`. In leap years write `אדר א` / `אדר ב`.
**Which Hebrew dates are after sunset?** Dates change at midnight (no sunset logic).
**Does dedupe delete my original data?** It rewrites the selected range with unique rows (Ctrl+Z undoes it). Select only the table you want deduped.
**Clean selection changed "00123" to 123.** Text-numbers are converted to numbers; exclude ID/ZIP columns from the selection.
**Custom functions slow?** They run per cell; use on ranges via ARRAYFORMULA: =ARRAYFORMULA(GREG2HEB(A2:A)).
**How do I uninstall?** Extensions → Add-ons → Manage add-ons.
