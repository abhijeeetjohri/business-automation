# 02 - AI Support Agent with Human-in-the-Loop

## The Business Problem
Businesses want to use AI to improve customer support response times, but they are terrified of "hallucinations"—AI models saying things that are factually incorrect or off-brand.

## The Solution
An "AI-Draft, Human-Approve" workflow. The system catches customer support tickets via Webhook, uses GPT-4o-mini to draft a professional response, and posts that draft to a private Slack channel. The support manager reviews the draft and approves it before it is ever sent to the customer.

## Key Features
- **Governance:** Ensures zero automated AI responses go to customers without human oversight.
- **Workflow Orchestration:** Demonstrates data passing between Webhooks, OpenAI, and Slack.
- **Human-in-the-Loop:** A core architectural pattern for safe enterprise AI.

## Tech Stack
- n8n (Workflow Engine)
- OpenAI API (GPT-4o-mini)
- Slack API (Notification & Approval)
