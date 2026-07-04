# 04 - Intelligent Booking Assistant

## The Business Problem
Scheduling meetings manually is a major bottleneck for sales teams. However, "naive" bots often double-book slots or fail to parse user input, leading to a poor customer experience.

## The Solution
An intelligent scheduling engine that parses natural language requests ("Tuesday at 2 PM") into standardized ISO timestamps and performs an availability check against a database before confirming the meeting.

## Key Features
- **Intelligent Parsing:** Uses a custom JavaScript Code Node to normalize human-readable time strings.
- **Availability Gate:** Prevents double-booking by enforcing a conditional logic gate before confirmation.
- **Workflow Reliability:** Ensures clear "True/False" paths for success and conflict handling.

## Tech Stack
- n8n (Webhook Triggers & Logic)
- JavaScript (Data Parsing/Normalization)
- Slack API (Automated Notifications)
