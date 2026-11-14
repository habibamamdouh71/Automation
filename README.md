# n8n Automation Projects

Four small workflows I built in n8n while learning automation. Each folder has the exported workflow (`workflow.json`) and screenshots of the nodes and the result.

| # | Project | What it does | Nodes |
|---|---------|--------------|-------|
| 1 | [Email notification](01-email-notification) | Sends me an email when someone submits a registration form | Webhook, Edit Fields, Gmail |
| 2 | [File to Google Sheets](02-file-to-google-sheets) | Downloads a CSV file and adds its rows to a Google Sheet | HTTP Request, Extract from File, Google Sheets |
| 3 | [Daily weather update](03-daily-weather-update) | Sends the weather report for Sohag to Telegram every morning | Schedule Trigger, HTTP Request, Telegram |
| 4 | [Social media post scheduler](04-social-media-post-scheduler) | Publishes a daily tip on LinkedIn at a fixed time | Schedule Trigger, Edit Fields, LinkedIn |

## How to import a workflow

1. Open n8n and create a new workflow.
2. Click the three dots in the top right, then **Import from File**, and pick the `workflow.json` of the project.
3. Credentials are not included in the export, so connect your own accounts in the Gmail, Google Sheets, Telegram and LinkedIn nodes.
4. Replace the placeholders (they all start with `YOUR_`) with your own values. Each project README lists which ones.

## Notes

- Never commit API keys or tokens. The workflow files here use placeholders.
- I used n8n cloud for the screenshots. The email project was also tested on a local n8n.
