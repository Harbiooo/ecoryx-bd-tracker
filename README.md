# Ecoryx Business Development Tracker

A self-contained, single-page tool for mapping professional connections to Saudi companies and tracking outreach progress for Ecoryx's sustainability advisory services.

## Live link

Once GitHub Pages is enabled, the tool is available at:
**`https://<your-github-username>.github.io/<repo-name>/`**

## What it does

- 124 Saudi companies grouped by 15 sectors (CBAM-relevant sectors highlighted)
- Each company shows English name, Arabic name, and website
- For each company, mark contact type (Direct / Indirect / None), priority, and context notes
- Track outreach through 5 stages: Introduction requested → Introduction completed → In discussion → Engaged → Closed
- Two views: Prospect list and Outreach pipeline (kanban-style)
- Export everything to CSV (UTF-8 with BOM, Excel-compatible)

## How data is stored

All data lives in the user's browser via `localStorage`. Nothing is sent to a server. Each user/device has its own state — there is no shared backend.

This means:
- The page works offline after first load
- The tracker is private to each device
- To merge the friend's input with Ecoryx's tracking, use the CSV export

## How to update

To edit the company list or the form itself:
1. Edit `index.html` directly in the GitHub web editor, or
2. Edit locally and commit/push the change

GitHub Pages will redeploy automatically within a minute.

## Files

- `index.html` — the entire app (HTML + CSS + embedded JS + embedded company data)
- `README.md` — this file

The app uses two external resources (Google Fonts and the Ecoryx logo from ecoryx.com) — both load on first visit and are cached.
