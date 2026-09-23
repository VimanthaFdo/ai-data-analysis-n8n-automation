
# AI Data Analysis & Email Automation (n8n)

An automated workflow that analyzes uploaded sales/business datasets using OpenAI 
and emails a formatted, easy-to-read business report — no manual analysis needed.

## How it works

1. **Form submission** — user uploads a CSV dataset via an n8n form
2. **Parse CSV** — converts the file into structured rows
3. **Data preprocessing** — cleans data, computes stats (sum, mean, min, max) per column
4. **AI analysis** — sends the dataset + stats to OpenAI, which returns a structured 
   business report (Executive Summary, KPIs, Trends, Issues, Recommendations)
5. **HTML email formatting** — converts the AI's markdown response into a styled, 
   professional HTML email (tables, headers, bullet points)
6. **Send email** — delivers the report via Gmail

## Tech used
- [n8n](https://n8n.io) (workflow automation)
- OpenAI API (Responses API / GPT model)
- Gmail API (email delivery)
- JavaScript (Code nodes for parsing, stats, markdown-to-HTML conversion)

## Setup
1. Import `ai-data-analysis-workflow.json` into your n8n instance
2. Add your own OpenAI and Gmail credentials
3. Update the form trigger and email recipient as needed

## Sample output
*(add a screenshot of your formatted email here)*
