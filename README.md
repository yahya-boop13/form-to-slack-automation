# Website Form → Slack Notification

Automatically posts a Slack notification the moment someone submits a website contact form. Built with [Make.com](https://make.com). Team gets pinged instantly so no lead slips through.

## See it in action
Live 30-second demo: https://www.loom.com/share/fcc3673bd14d45b2947fd282bd88f069

## What it does
When a visitor submits the contact form, their **name, email, and message** are posted straight to a chosen Slack channel in real time.

## How it works
```mermaid
flowchart LR
    A[Website form submitted] --> B[Make.com webhook catches the data]
    B --> C[Slack message posted to channel]
```

## What the Slack message looks like
```
🔔 New form submission!

👤 Name: Jane Doe
📧 Email: jane@company.com
💬 Message: I'd like to book a call
```

## Stack
- **Make.com** for the automation
- **Slack** for notifications
- Works with any web form: Typeform, Webflow, WordPress/Elementor, or custom HTML

## Setup overview
1. Create a Make.com scenario with a Custom Webhook trigger
2. Point the website form at the webhook URL
3. Add a Slack "Create a Message" action and map the fields
4. Turn the scenario on

## Files
- `form.html`: a sample contact form that posts to a Make.com webhook

Built by Yahya. Available for automation work.
