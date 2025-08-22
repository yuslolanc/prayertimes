# Masjid al Noor • Prayer Times (Kiosk)

A single-file kiosk page that reads `prayertime.csv` from the same folder and shows **today's Jama'ah times**,
**tomorrow's column**, a **next prayer countdown**, and **Friday Jumu'ah 1/2** paired side by side.

## How to use

1. Put these three files at the repo root:
   - `index.html`
   - `prayertime.csv`
   - `logo.png` (optional)

2. Enable GitHub Pages (Settings → Pages → Deploy from branch).

3. Edit `prayertime.csv` on GitHub any time. Reload the page (or click **Refresh**) to pull the latest.
   The page fetches with `cache: no-store` and a cache-busting query.

### CSV headers

Required columns (case-insensitive, flexible naming for iqamah/jamaat):
- `date` (e.g., `2025-08-21` or `21/08/2025`)
- `fajr_iqamah`, `dhuhr_iqamah`, `asr_iqamah`, `maghrib_iqamah`, `isha_iqamah`
- `jumuah1`, `jumuah2` (used for Fridays)

Extra columns are ignored.

