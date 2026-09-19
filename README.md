# AI Business Automation Platform — Version 3

An AI-powered customer support and sales automation platform built with n8n, Telegram, Groq, and Supabase.

## What This Project Does

This automation allows customers to interact with an AI business assistant through Telegram.

The assistant can:

* Answer customer questions
* Remember conversation context
* Look up business products and services
* Register new customers
* Prevent duplicate registrations
* Send registration confirmation emails
* Create sales leads
* Record customer budgets and interests
* Schedule appointments
* Log conversations
* Escalate customers who request human assistance

## Technology Stack

* n8n
* Telegram Bot API
* Groq AI
* Supabase
* PostgreSQL
* Gmail
* AI Agent
* JavaScript expressions

## Workflow

Customer
↓
Telegram
↓
Telegram Trigger
↓
Edit Fields
↓
AI Agent
↓
Groq Chat Model
↓
Supabase / Gmail Tools
↓
Edit Fields
↓
Telegram Response

## Database

The project uses Supabase/PostgreSQL with the following tables:

* customers
* products
* leads
* conversations
* appointments

## Main Features

### Customer Registration

The AI collects:

* Full name
* Phone number
* Email

The customer's Telegram ID is automatically captured.

### Product Information

The AI retrieves products and services directly from the Supabase database.

### Lead Management

When a customer shows genuine buying interest, the AI can create a lead containing:

* Customer
* Product/service interest
* Budget
* Intent
* Status
* Source

### Appointment Scheduling

Customers can request appointments.

The AI collects the appointment date and time before creating the appointment in Supabase.

### Conversation Logging

Customer conversations can be stored in the database for future reference.


## Security

This repository does not contain API keys, passwords, access tokens, or other private credentials.

Credentials are configured separately inside n8n.

## Project Status

Version 3 — Completed learning project.

Additional production features such as owner notifications, appointment approval automation, advanced error handling, and security hardening can be added in future versions.

## Author

Prince Digital Solutions
