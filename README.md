# Dr. Meenu Sharma Fullstack Website

Express/Node version of the appointment website with a real email API powered by Nodemailer.

## Local setup

```bash
npm install
cp .env.example .env
npm run dev
```

Open `http://localhost:3000`.

## Email setup

For Gmail, enable 2-Step Verification, create a Gmail App Password, and use it as `SMTP_PASS`.

Required environment variables:

```bash
SMTP_HOST=smtp.gmail.com
SMTP_PORT=465
SMTP_SECURE=true
SMTP_USER=your-gmail-address@gmail.com
SMTP_PASS=your-gmail-app-password
MAIL_TO=mentalhealthsolutions01@gmail.com
MAIL_FROM="Dr. Meenu Sharma Website <your-gmail-address@gmail.com>"
```

## Deploy on Render

1. Push this folder to GitHub.
2. Create a new Render Web Service from the repository.
3. Use:
   - Build command: `npm install`
   - Start command: `npm start`
4. Add the environment variables from `.env.example`.

The included `render.yaml` can also be used as a Render blueprint.

## Deploy on Railway

1. Push this folder to GitHub.
2. Create a Railway project from the repository.
3. Add the same environment variables.
4. Railway will run `npm start` automatically.
