# Medicus Patient Record Visualiser

A single-file offline clinical tool for visualising Medicus EPR patient record exports. Drop a PDF in. Everything runs in the browser. Nothing leaves your machine.

---

## Download

**[Download visualiser.html](https://github.com/davetriska02-collab/medicus-record-visualiser/releases/latest/download/visualiser.html)**

That's it. One file. ~2MB. No installer, no admin rights, no dependencies.

---

## How to use

1. Download `visualiser.html`
2. Save it anywhere — desktop, USB drive, network share
3. Open it in Chrome, Edge, or Firefox
4. Drop a Medicus patient record PDF onto the page

The file works entirely offline. No internet connection required after download. No data is ever transmitted anywhere.

---

## What it shows

### Dashboard
- Summary stat cards (contacts, prescriptions, referrals, investigations)
- **Attendance Velocity** — contact rate trend across three time periods (early / mid / recent)
- **Gaps in Care** — flags statistically unusual gaps between consultations (mean + 2SD, minimum 180 days)
- **Complexity Score** — 0–100 composite score across contact volume, prescriptions, referrals, investigations, clinician diversity, and record span
- Referral breakdown — click the Referrals card to see destination breakdown and dated list
- Contacts per year bar chart + entry type donut chart

### Timeline
- Full chronological scatter plot of all entries, filterable by type and date range
- **Safeguarding Chronology** — one-click panel showing all safeguarding-flagged entries in date order
- **Problem-linked filtering** — click any cell in the Problems heatmap to filter the timeline to related entries; badge shows active filter

### Contact Rates
- Stacked bar chart by year and entry type
- Year-by-year breakdown table
- Clinician frequency table — click any name to filter the timeline to their entries
- **Clinician Continuity Index** — UPC (Usual Provider of Care) and CPCI (Consecutive-pair continuity) metrics

### Clinician Continuity
- D3 heatmap of contacts per month per clinician
- Colour intensity shows frequency

### Investigations
- Stat cards (total, unique types, date range)
- Investigations per year chart
- Category and record-type breakdown
- Searchable entry list

### Problems & Medications
- Problems activity heatmap (years × problems) — click a cell to filter the Timeline
- New problems per year bar chart
- Raw problems summary text
- Searchable prescription list
- **Medication Timeline** — D3 Gantt chart of top 20 drugs plotted across the record period

### Letters & Correspondence
- Yearly chart of correspondence volume
- Stat cards (total, secondary care letters, most recent, distinct authors)
- Filterable list by year and record type

### Global
- **Full-text search** — press `Ctrl+K` (or `⌘K` on Mac) to search across all record entries; matches are highlighted
- **Export Summary** — click the Export button in the header to open a print-ready summary page (patient banner, overview stats, top clinicians, 10 most recent entries)

---

## Compatibility

| Browser | Status |
|---------|--------|
| Chrome 90+ | Supported |
| Edge 90+ | Supported |
| Firefox 88+ | Supported |
| Safari 15+ | Supported |

Does not require any browser extensions, plugins, or elevated permissions.

---

## Information governance

- All processing is local. The PDF is parsed entirely in the browser using an embedded pdf.js library.
- No data is sent to any server, API, or third party at any point.
- Closing the browser tab clears all data from memory.
- The tool does not write to disk, set cookies, or use localStorage.
- Suitable for use with identifiable patient data on NHS-managed devices under existing IG policies for locally-run clinical tools.

---

## Source

Built by [Dr Dave Triska](https://davetriska.substack.com), GP Partner at Witley & Milford Surgery, as part of the DHSC 10-year programme with Medicus and Surrey Heartlands ICB.

Libraries bundled inline: [pdf.js](https://mozilla.github.io/pdf.js/) · [D3.js v7](https://d3js.org/) · [Chart.js](https://www.chartjs.org/)
