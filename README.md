# Follow-up Tracker

Automatically checks a Google Sheet on a schedule and sends follow-up emails to leads that meet a certain condition (e.g. no response yet) — then updates the sheet so the same lead isn't followed up with twice.

## How it works

1. **Schedule Trigger** — Runs automatically at set intervals (e.g. daily)
2. **Get row(s) in sheet** — Reads all leads from the connected Google Sheet
3. **If** — Checks a condition (e.g. "has this lead been followed up with yet?")
   - **True** → Sends a follow-up email and updates the sheet
   - **False** → Skips the lead
4. **Send a message** — Sends the follow-up email via Gmail
5. **Update row in sheet** — Marks the lead as followed up, so they aren't emailed again

## Why it matters

Following up with leads manually is easy to forget and hard to track consistently. This automation runs on its own schedule, checks who needs a nudge, and handles the follow-up — so no lead is missed and no one gets emailed twice.

## Built with

- [n8n](https://n8n.io) — workflow automation
- Google Sheets
- Gmail

## Setup

1. Clone this repo
2. Import the workflow JSON into your n8n instance
3. Connect your Google Sheets account (OAuth)
4. Connect your Gmail account (OAuth)
5. Adjust the schedule and follow-up condition to fit your needs
6. Activate the workflow

## License

MIT
