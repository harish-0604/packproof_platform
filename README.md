# Pack Proof -- SCAN. VERIFY. PROTECT.

> **Smart Legal Metrology Compliance System for India**
> SIH 2026 | Problem Statement ID: **SIH26034**
> Ministry of Consumer Affairs, Food & Public Distribution
> Legal Metrology (Packaged Commodities) Rules, 2011

---

## Live Demo

[Open Live App](https://delicate-eclair-558474.netlify.app)

---

## Team PHANTOM SYNDICATE

| Member | Role |
|--------|------|
| Member 1 | AI/ML & Compliance Engine |
| Member 2 | Frontend PWA Development |
| Member 3 | Legal Metrology Research |
| Member 4 | UI/UX & Data Visualization |
| Member 5 | Backend & Deployment |
| Member 6 | Testing & Documentation |

---

## Problem Statement

India's current packaged commodity inspection system relies on **manual, paper-based** processes. This leads to:

- MRP overcharging and dual-MRP fraud
- Shrinkflation (net weight reductions without price change)
- Missing mandatory declarations (FSSAI, BIS, Mfg/Exp date)
- Font size violations (less than 1.5mm for critical information)
- No real-time compliance evidence trail for Legal Metrology Officers

---

## Our Solution

A **single-file Progressive Web App (PWA)** that gives Legal Metrology Officers and citizens an AI-powered compliance checking tool.

### Core Features

| Feature | Description |
|---------|-------------|
| OCR Scanner | Tesseract.js-powered text extraction from label images |
| Barcode/QR Reader | jsQR live camera scanning |
| Compliance Engine | 47 rules from PCR 2011 checked automatically |
| Dashboard | Executive Command Centre with live KPIs |
| Inspection Reports | Auto-generated PDF dossiers with evidence |
| Shrinkflation Tracker | Historical net-weight monitoring |
| Citizen Bounty Portal | Crowdsourced violation reporting |
| Offline Mode | Full PWA -- works without internet |

### 3 Deployment Modes

```
Mode A -- Retail Shelf Sweep    : Live webcam continuous scanning of shelves
Mode B -- Single Product Check  : Detailed per-item compliance audit
Mode C -- Bulk Import           : CSV/Excel batch processing for warehouses
```

---

## Architecture

```
+---------------------------------------------+
|           Pack Proof PWA (index.html)        |
|  +----------+ +----------+ +-------------+  |
|  | Camera   | |   OCR    | |  Compliance |  |
|  | Module   | | Engine   | |   Engine    |  |
|  | (jsQR)   | |(Tesseract| |  (47 Rules) |  |
|  +----------+ +----------+ +-------------+  |
|  +--------------------------------------+    |
|  |         State Management             |    |
|  |    (localStorage - offline-first)    |    |
|  +--------------------------------------+    |
+---------------------------------------------+
```

**Tech Stack:**
- Frontend: Vanilla JS + HTML5 + CSS3 (zero frameworks)
- OCR: Tesseract.js v5 (CDN)
- Barcode: jsQR (CDN)
- PDF Export: jsPDF (CDN)
- Excel Export: SheetJS/XLSX (CDN)
- Storage: localStorage (offline-first PWA)
- Hosting: Netlify

---

## Run Locally

### Option 1 -- Double Click (Windows)
```
Double-click START_SERVER.bat
```
Opens automatically at http://127.0.0.1:8080

### Option 2 -- Python
```bash
cd "D:\PHANTOM SYNDICATE"
python -m http.server 8080
```
Then open: http://127.0.0.1:8080

### Option 3 -- Direct File
Just open `index.html` in Chrome or Edge
*(Note: Camera features require localhost for full functionality)*

---

## Repository Structure

```
packproof-sih2026/
|-- index.html                              <- Entire PWA (single file)
|-- packproof_logo.png                      <- App shield logo
|-- START_SERVER.bat                        <- Local server launcher
|-- architecture_mild.png                   <- System architecture diagram
|-- architecture_flowchart.png              <- Data pipeline flowchart
|-- diagram_problem_solution.png            <- Problem/Solution overview
|-- innovations_diagram.png                 <- 6 core innovations
|-- two_tier_diagram.png                    <- Two-tier deployment model
|-- packproof_sih_infographic.jpg           <- SIH submission infographic
|-- Pack_Proof_Complete_Project_Report.pdf  <- Full 12-page project report
|-- SIH2026_PackProof_Official_Submission.pdf   <- SIH official submission
|-- SIH2026_PackProof_Official_Submission.pptx  <- Presentation slides
```

---

## Legal Framework Covered

Pack Proof enforces compliance with:

- **Rule 6** -- Mandatory declarations (name, net qty, MRP, Mfg date)
- **Rule 22** -- MRP display and format requirements
- **Rule 24** -- Font size minimums (1.5mm for critical info)
- **Rule 26** -- Net quantity tolerance limits
- **Schedule II** -- Commodity-specific weight/measure rules

---

## Impact

- 8.5 Cr+ retail outlets in India can be monitored
- 7,500+ Legal Metrology Officers empowered
- 140 Cr consumers protected from overcharging
- Inspection time reduced from ~45 min to ~8 min per product

---

## License

This project was developed for **Smart India Hackathon 2026**.
All rights reserved -- Team PHANTOM SYNDICATE.

---

*Built with love for India's consumers*

