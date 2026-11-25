# W4-D1 — n8n AI Agent for Gmail

**Unread Email Summariser**: an n8n workflow that fetches the latest 5 unread Gmail messages, asks an AI Agent to describe each one in a single line (max 20 words), combines the summaries, and emails them back as one message.

## Workflow
Manual Trigger → Gmail (Get Many, Unread, Limit 5) → AI Agent (+ OpenAI Chat Model) → Aggregate (`output`) → Gmail (Send)

## Files
- `Week4_Day1_n8n_Gmail_AI_Agent.pdf` — assignment brief
- `Unread_Email_Summariser.json` — exported n8n workflow (import via *Import from File*)
- `workflow-screenshot.png` — workflow canvas

## Setup after import
1. Select your Gmail OAuth2 credential on both Gmail nodes.
2. Select your OpenAI credential on the chat model node.
3. Set your own address in the **Send Summary Email** node.
