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

Email Body
Dear [Name],

This is a friendly reminder that your payment for Invoice ID:
[Invoice ID] of Amount: ₹[Amount] is currently pending.

Please find your payment details below for reference:

Account No: [Account No]
Bank Name: [Bank Name]
Payment Type: [Type]
Transaction ID: [Transaction ID]

Kindly ensure the payment is completed at the earliest to avoid any inconvenience.

If you have already made the payment, please disregard this message.

Thank you for your cooperation.

Regards,
Payments Team

## Input Data Structure

The workflow uses the following fields from the `SCIT Invoice` spreadsheet:

| **Field** | **Purpose** |
|---|---|
| **Sr** | Serial/reference number |
| **Invoice ID** | Unique identifier of the invoice |
| **Type** | Payment or invoice type |
| **Name** | Name used to personalize the email |
| **Amount** | Invoice/payment amount |
| **Account No** | Bank account reference |
| **Bank Name** | Bank associated with the record |
| **Status** | Current payment status |
| **Transaction ID** | Transaction reference when available |
| **Reminder Count** | Number of reminders already issued |
| **Escalated** | Indicates whether the record has been escalated |
| **Email** | Designated test recipient address |

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
