# AI Career Guide

This repository contains the AI Career Guide marketing website and a Node.js backend to support the Contact Us form.

## Contact Us Feature

- A **Contact Us** button opens a modal form.
- The form includes Name, Phone Number, Email, Recipient email selection, and Message fields.
- The form uses client-side validation and submits via AJAX to the backend.
- The backend sends the message to the chosen email address using SMTP.

## Setup

1. Copy `.env.example` to `.env` and fill in your SMTP credentials.
2. Run `npm install` to install dependencies.
3. Start the app with `npm start`.
4. Visit `http://localhost:3000` in your browser.

## Backend endpoints

- `POST /api/contact` — accepts JSON payload with `name`, `phone`, `email`, `recipientEmail`, and `message`.

## Notes

- Allowed recipient emails are hard-coded to the two emails already listed in `index.html`.
- Use a valid SMTP account and credentials in `.env` to enable email delivery.
- If your SMTP provider uses a self-signed certificate, add `EMAIL_TLS_REJECT_UNAUTHORIZED=false` to `.env`.
# ai-career-guide
