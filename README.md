# Automated Payment Reminder System using Zapier
https://agents.zapier.com/copy/65c3ba40-b434-45e2-9a65-0150659df063

Google sheet link - 
https://docs.google.com/spreadsheets/d/1C8QezSuCf7yhpllobUne75CGsOU9IA417mUSJmodt6U/edit?usp=sharing

# Automated Payment Reminder System using Zapier

## Project Overview

This project demonstrates an automated payment reminder workflow developed using Zapier, Google Sheets, and Gmail.

The system retrieves invoice records from a spreadsheet, identifies pending payments, and sends personalized payment reminder emails to designated test recipients. After sending the reminder, the spreadsheet is updated to record the reminder status.

## Objective

The objective is to automate the manual process of identifying pending payments and sending payment reminder emails.


The workflow demonstrates:

- Scheduled automation
- Spreadsheet data retrieval
- Conditional filtering
- Dynamic data mapping
- Automated email delivery
- Spreadsheet updates
- Reminder tracking

## Tools and Technologies

- Zapier
- Google Sheets
- Gmail
- Google Drive
- CSV / Excel

## Workflow

```text
Schedule by Zapier
        ↓
Google Sheets – Get Many Spreadsheet Rows
        ↓
Filter – Status = Pending
        ↓
Filter – Email Exists
        ↓
Gmail – Send Payment Reminder
        ↓
Google Sheets – Update Spreadsheet Row
