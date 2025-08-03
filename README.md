# Tally to Google Sheets & Gmail Lead Automation
This repository contains a **Make.com scenario** that automates lead capture from Tally forms, processes data, logs it to Google Sheets, and sends instant Gmail notifications. It showcases expertise in **workflow automation, API integration, data processing, Google Sheets integration, and email automation**, delivering efficient lead management for agents, small businesses, and entrepreneurs.

---

## Project Overview

The workflow captures Tally form submissions (`name`, `email`, `company`, `automation goal`, `urgency`), processes them using Make.com’s **Webhook, Iterator, and Array Aggregator** modules, logs structured data to Google Sheets, and triggers immediate personalized Gmail emails. **Error-handling filters** ensure reliability, making it ideal for streamlining lead management.

---

## Features

- Captures Tally form fields: Name, Email, Company, Automation Goal, Urgency.
- Logs data to Google Sheets with columns: Timestamp, Name, Email, Company, Automation Goal, Urgency, Lead Status.
- Sends instant, personalized Gmail notifications to leads.
- Implements error-handling filters for robust data processing.
- Demonstrates scalable automation for business workflows.

---

## Technologies Used

- **Make.com**: Workflow automation with Webhook, Iterator, Array Aggregator.
- **Tally**: Form creation and submission.
- **Google Sheets**: Data storage and logging.
- **Gmail**: Automated email notifications.
- **JSON**: Data mapping and processing.

## Setup Instructions

### 1. Import Scenario
- Log in to Make.com.
- Navigate to **Scenarios > Create a new scenario > Import Blueprint**.
- Upload `scenario.json` from this repository.

### 2. Configure Modules
- **Webhook:** Link a Tally form to the Webhook URL.
- **Google Sheets:** Connect your Google account, select the target spreadsheet/tab, and map fields (e.g., `{{3.array[1].value}}` for Name, `{{3.array[5].options[].text}}` for Urgency).
- **Gmail:** Connect your Gmail account and set the email template (e.g., To: `{{3.array[2].value}}`, Subject: Hi `{{3.array[1].value}}`, Let’s Automate!).

### 3. Test Workflow
- Submit a Tally form.
- Verify Google Sheets data (Timestamp, Name, Email, Urgency, etc.).
- Confirm Gmail email delivery.

- Building **scalable lead management solutions** adaptable to various business needs.
