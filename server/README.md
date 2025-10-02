# Nadhari Contact Form Server

This is a Node.js Express server for handling contact form submissions and sending emails via Gmail SMTP.

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```
2. Create a `.env` file in the `server` directory with:
   ```env
   GMAIL_USER=yourgmail@gmail.com
   GMAIL_PASS=yourapppassword
   MAIL_TO=yourdestination@email.com
   ```
   - Use a Gmail App Password (not your main password).

3. Start the server:
   ```bash
   npm start
   ```

## API Endpoint
- `POST /api/contact`
  - Body: `{ firstName, lastName, email, phone, subject, message }`

## Deployment
- For production, deploy to a Node.js-friendly cloud (Render, Vercel, DigitalOcean, etc.).
- Update environment variables as needed.
