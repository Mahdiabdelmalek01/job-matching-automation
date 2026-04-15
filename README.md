# AI Job Matching Automation

Automated LinkedIn job scraping and AI-powered matching system built with n8n.

## How it works
1. Apify scrapes LinkedIn jobs daily based on keywords
2. Google Gemini scores each job against my candidate profile (1-10)
3. High-scoring jobs (≥7) trigger a Telegram notification
4. All jobs logged to Google Sheets with score, reason and status tracking

## Tech Stack
- n8n (workflow automation)
- Apify (LinkedIn scraping)
- Google Gemini API (AI scoring)
- Google Sheets (tracking)
- Telegram Bot API (notifications)

## Workflow Screenshot
<img width="879" height="463" alt="Screenshot 2026-04-15 at 13 56 17" src="https://github.com/user-attachments/assets/f1837bd0-8f08-462b-b6d8-bd73d63c7d1b" />
