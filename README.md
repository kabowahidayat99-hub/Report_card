# Report_card

README – KABOWA HIDAYAT ISLAMIC PRIMARY SCHOOL

Electronic Report-Card Generator (KReport.html)

1. WHAT IT IS

A single-file, zero-dependency (except the two CDN scripts) HTML page that turns any phone, tablet or PC into a fully-fledged Ugandan-primary report-card printer.

Open → type → click “Calculate” → click “Save as PDF”.

That is the whole workflow.

2. FEATURES

• Dual-language interface – secular subjects in English, Islamic subjects in Arabic.

• Automatic aggregates, division, position, promotion status and teacher comments.

• Instant print stylesheet – margins, page-breaks and colours optimised for A4.

• One-tap PDF export – file name auto-generated: `Aisha_Namusoke_P6_Term1_2025.pdf`.

• Offline capable – once the page is saved, it works without internet (only PDF creation needs the two cached CDN files).

• Responsive – runs in a mobile browser; no app store, no installation.

• Secure – no data leaves the device; everything happens in the browser.

3. QUICK START  
1. Save `KReport.html` to any folder.  
2. Double-click to open in Chrome, Edge, Safari or Opera.  
3. Fill the white cells (marks) → blue “Calculate Results” button.  
4. Red “Save as PDF” button → file drops in your “Downloads” folder.  
5. Hand the printed A4 sheet to parent/guardian.

4. CUSTOMISING FOR YOUR SCHOOL

a) Logo / Student photo – click the placeholder image, pick any JPG/PNG.

b) Subjects – edit the four arrays at the top of the script:

   `lowerSecular`, `upperSecular`, `arabicSubjects`.

c) Grading scale – functions `getAggregate`, `getSecularRemark`, `getArabicRemark`.

d) Comments – objects `classTeacherComments`, `dosComments`, `htComments`.

e) Motto – change the text inside `<div class="motto">`.

f) Colours – replace any `#006400` with your theme colour.

5. FILE STRUCTURE

Only one file is required:

`KReport.html` – contains HTML, CSS and JavaScript in a single bundle.

6. DEPENDENCIES (loaded from CDN, cached after first use)

• html2canvas 1.4.1 – rasterises the page.

• jsPDF 2.5.1 – packages the image into a PDF.

7. TROUBLE-SHOOTING

• PDF button does nothing → use a modern browser (Chrome 90+, Safari 14+, Edge 90+).

• Arabic text mis-aligned → ensure `dir="rtl"` is kept on the Arabic table.

• Photo disappears after reopening → images are embedded on-the-fly; to keep them permanently, convert the file to PDF immediately.

• Print preview cuts off → choose “A4” and “Margins: Default” in the print dialog; the CSS already sets 10 mm padding.

8. LICENCE

Public domain – do whatever you want: use it, fork it, sell it, no attribution required.

9. ROAD-MAP IDEAS (not implemented)

• LocalStorage auto-save so you can close the browser and resume later.

• Bulk generator (loop over a CSV of names & marks).

• Dark-mode toggle.

• Swahili remark set.

Pull requests welcome – the code is intentionally kept flat and readable.

10. NEED HELP?

Open an issue on your favourite pastebin/Git repo or e-mail the ICT master who gave you this file.

Remember: everything happens in the browser – no student data is ever sent anywhere.