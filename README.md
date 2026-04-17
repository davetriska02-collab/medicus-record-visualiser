# Medicus Patient Record Visualiser

> Drop a Medicus PDF onto one file. Get a searchable, visual patient record in your browser. Nothing leaves your computer.

Made for GPs, practice managers, safeguarding leads, and clinical reviewers who want a fast way to see what's actually in a long patient record — without installing anything, without sending data anywhere, and without needing any technical skills.

---

## Download

### **[Click here to download the visualiser](https://github.com/davetriska02-collab/medicus-record-visualiser/releases/latest/download/visualiser.html)**

One file. About 2 MB. No installer. No admin rights. No sign-up.

---

## How to use it (3 steps)

1. **Download** the file above. It's a single `.html` file — save it to your desktop, Documents, a USB stick, or a shared drive. Wherever is convenient.
2. **Open it** by double-clicking. It opens in your usual browser (Chrome, Edge, Firefox, Safari — they all work).
3. **Drop a PDF** onto the page. A Medicus patient record export is what it's designed for.

That's it. The whole patient record becomes interactive in a few seconds.

If your browser asks whether you trust the file — yes, it's just an HTML page. It's not an executable, doesn't install anything, and can't change anything on your computer.

---

## What you get

### At a glance
- **Dashboard** — headline stats, years covered, top clinicians, contact type breakdown
- **Complexity Score** — a 0–100 score summarising how involved a patient's care has been
- **Attendance Velocity** — is this patient's contact rate rising, falling, or steady over time?
- **Gaps in Care** — highlights unusually long gaps between consultations
- **Clinician Continuity Index** — measures how consistent a patient's care team has been

### Deep-dive views
- **Timeline** — every entry plotted chronologically. Filter by type, date range, or clinician. Click any point for full detail.
- **Safeguarding Chronology** — one-click view of all safeguarding-flagged entries in date order
- **Investigations** — blood tests, imaging, and reports, with a yearly trend chart
- **Prescriptions** — searchable list and medication timeline (Gantt chart of the top 20 drugs)
- **Problems & Medications** — activity heatmap showing which problems flared up in which years
- **Letters & Correspondence** — hospital letters, clinic outcomes, discharge summaries
- **Patient Comparison** — load a second patient and compare them side-by-side (useful for siblings, household members, or audit)

### Tools always at hand
- **Floating toolbar** — sits in the corner on every view. Pin it where you like.
- **Copy Summary** — one click copies a plain-text summary to your clipboard. Paste it into EMIS, an email, or a referral letter.
- **Search** — `Ctrl+K` (or `⌘K` on Mac) to search the entire record with highlighted matches.
- **Export any chart as an image** — hover over a chart and click the download button to save it as a PNG for meeting notes, MDT discussions, or reports.

---

## Why it's safe to use with real patient data

- **Nothing is sent anywhere.** The file is entirely self-contained. It has no internet access, no analytics, no tracking.
- **Nothing is saved.** Closing the browser tab clears everything. No cookies, no local storage, no disk writes.
- **All processing happens in your browser** using PDF-reading code that runs inside the page itself.
- Suitable for use on NHS-managed devices under existing IG policies for locally-run clinical tools.

If you want to audit the code, it's all in the single HTML file — open it in any text editor and read through.

---

## Browser compatibility

| Browser | Supported |
|---------|-----------|
| Chrome 90+ | ✓ |
| Edge 90+ | ✓ |
| Firefox 88+ | ✓ |
| Safari 15+ | ✓ |

No extensions, no plugins, no elevated permissions required.

---

## Questions or problems?

- Open an [issue on GitHub](https://github.com/davetriska02-collab/medicus-record-visualiser/issues) — tell me what went wrong, what browser you're using, and roughly what was in the PDF (no patient details please).
- Feature requests welcome.

---

## About

Built by [Dr Dave Triska](https://davetriska.substack.com), GP, as part of the DHSC 10-year programme with Medicus and Surrey Heartlands ICB.

Libraries bundled inline: [pdf.js](https://mozilla.github.io/pdf.js/) · [D3.js v7](https://d3js.org/) · [Chart.js](https://www.chartjs.org/)
