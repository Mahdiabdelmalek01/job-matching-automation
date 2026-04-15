# AI Job Matching Automation

Automated LinkedIn job scraping, AI-powered matching and personalized motivation 
letter generation system built with n8n.

## How it works
1. Apify scrapes LinkedIn jobs daily based on keywords (Werkstudent, KI, Consulting)
2. Google Gemini scores each job against my candidate profile (1-10)
3. For high-scoring jobs (≥7), Gemini automatically generates a personalized 
   motivation letter in German
4. Job alert + motivation letter sent instantly via Telegram
5. All jobs logged to Google Sheets with score, reason and status tracking

## Tech Stack
- n8n (workflow automation)
- Apify (LinkedIn scraping)
- Google Gemini API (AI scoring + letter generation)
- Google Sheets (job tracking)
- Telegram Bot API (notifications)

## Workflow
<img width="867" height="393" alt="Screenshot 2026-04-15 at 14 45 01" src="https://github.com/user-attachments/assets/758c779a-8315-4b67-ae96-fba3fb4c5e6b" />


## Setup
1. Import `workflow.json` into your n8n instance
2. Add your credentials:
   - Apify API Token
   - Google Gemini API Key
   - Google Sheets OAuth
   - Telegram Bot Token + Chat ID
3. Update the LinkedIn search URLs in the Apify node
4. Update the candidate profile in the Gemini prompt
5. Activate the workflow

## Output Example
- Google Sheets: job title, company, location, AI score, match reason, link, status
- Telegram: instant notification with score, match reason and ready-to-use 
  motivation letter
