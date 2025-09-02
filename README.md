# Customer Onboarding Automation with n8n

Automates new customer onboarding using HubSpot, email sequences, and team notifications.

## Features
- Receives signup data via webhook
- Validates customer info
- Creates a contact in HubSpot CRM
- Sends personalized welcome email
- Sends onboarding documents after 2 hours
- Sends personal check-in email after 1 day
- Sends Week 1 success guide after 3 days
- Updates CRM and notifies team at each milestone

## Setup Steps
1. Create Webhook in n8n (POST method)
2. Add IF node to validate email and customerName
3. Use HubSpot node to create CRM contact
4. Add Telegram/Slack node for team alerts
5. Use Email Send node for welcome and onboarding emails
6. Add Wait nodes for timed delivery
7. Update CRM and notify team on completion
