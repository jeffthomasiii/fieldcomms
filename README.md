# FieldComms

**Radio • Plans • Preparedness**

An offline-oriented, browser-based radio reference and communications preparedness planner. FieldComms does **not** program radios, modify CHIRP/CPS files, grant transmission authorization, verify licenses or certify regulatory compliance.

## Live application

Once GitHub Pages is enabled for **main / (root)**: https://jeffthomasiii.github.io/fieldcomms/

## MVP features

- Forest / olive / warm ivory / restrained amber responsive dashboard and mobile navigation
- Manual radio registration
- Read-only import of existing CHIRP-style CSV files, with `Location` and `Frequency` headers
- Associate imported records with radio profiles; search names, frequencies, comments and memories
- Activity-specific planning: camping, hiking, events, outings, road trips and emergency preparedness
- Primary/alternate channel selection from uploaded records
- Field-card print preview and browser **Print → Save as PDF**
- Local browser persistence plus JSON backup/restore
- Operator responsibility notice and official FCC/NOAA resource links

## Getting started

1. Open the Pages site, or launch `index.html` locally in a modern browser.
2. Add a radio under **Radios**.
3. Export a CHIRP CSV from your own separately managed programming software and import it under **Channels**.
4. Select an activity under **Plans**, choose imported channel labels and save the plan.
5. Open **Field Guides** and print a PDF using the browser.

The application currently uses `localStorage` for data. Browser storage is limited and device/browser-specific; **export JSON backups** under Settings. There is no server account, remote upload or required API key.

## Source and usage boundaries

Imported CSV values are displayed as originally supplied for informational use. A channel's presence in an import does not imply that a transmission is lawful, that access to a repeater is authorized, or that a given device can transmit on that frequency. FieldComms never exports a modified CHIRP file or connects to radios. Do not upload private family details or live radio programming backups into the public GitHub repository.

NOAA weather listening is not equivalent to automatic SAME emergency alerting. An ordinary GMRS handheld is not a substitute for an emergency communications service. Emergency plans must prioritize safe action, appropriate official alerts, and working emergency contact methods.

## Operator responsibility

Every operator is solely responsible for equipment, licensing, regulations, frequencies, emissions, repeater permissions and all other applicable legal and operational requirements. FieldComms is educational reference software, not a compliance check, license verifier, safety certification or emergency dispatch tool. Independently verify information and operating conditions.

- [FCC GMRS rules](https://www.ecfr.gov/current/title-47/chapter-I/subchapter-D/part-95/subpart-E)
- [FCC FRS rules](https://www.ecfr.gov/current/title-47/chapter-I/subchapter-D/part-95/subpart-B)
- [FCC amateur rules](https://www.ecfr.gov/current/title-47/chapter-I/subchapter-D/part-97)
- [NOAA Weather Radio](https://www.weather.gov/nwr/)

## Design standard

- Forest `#17362e`
- Olive `#687b41`
- Warm ivory `#f5f1e9`
- Amber `#b97830`
- Georgia editorial headings, system sans-serif body
- Responsive desktop sidebar and small-screen bottom navigation
- Print-friendly half-page/one-page references

## Remaining MVP acceptance tests

- Validate a real, backed-up CHIRP CSV import without making any radio changes
- Confirm imported memory numbers, commas in quoted fields, row counts and associated radio profile
- Verify a plan's primary/backup channels match the actual physical radio
- Confirm printing in Chrome, Edge and mobile browsers
- Test JSON restore in a fresh browser profile
- Test layout at 375px mobile and desktop widths

**Current maturity:** initial directly committed MVP implementation; not yet device or browser field validated.

## License

MIT. See [LICENSE](LICENSE).
