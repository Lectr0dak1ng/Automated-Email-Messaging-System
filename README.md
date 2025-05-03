Python Email Sender with Attachments and Images

This project provides a simple Python script to send emails with plain text, images, and attachments using Gmail SMTP and the smtplib and email libraries.

✅ Features
Send emails using a Gmail account

Supports multiple recipients

Optionally attach:

Plain text

Images (e.g., .jpg, .png)

Any file type (e.g., .pdf, .docx, .zip)

Secure connection using TLS

🐍 Requirements
Python 3.x

Internet access

Enabled "Less Secure Apps" or App Passwords in your Gmail account settings (recommended for Gmail)

🛠️ Setup & Usage
Install Python (if not already installed)

Edit Your Gmail Credentials
Replace the placeholders in the script:

python
Copy
Edit
smtp.login('your_email@gmail.com', 'your_password_or_app_password')
⚠️ Important: Using a regular password is discouraged. Instead, generate an App Password in your Google account for better security.

Define Email Content

python
Copy
Edit
msg = message("Subject", "Your message text here", img="image.jpg", attachment="file.pdf")
Specify Recipients

python
Copy
Edit
to = ["recipient1@example.com", "recipient2@example.com"]
Run the Script

bash
Copy
Edit
python email_sender.py
📂 Project Structure
bash
Copy
Edit
email_sender.py   # Main script
image.jpg         # Optional: Example image
file.pdf          # Optional: Example attachment
README.md
🔐 Security Notes
Use App Passwords for Gmail. You can generate one at: https://myaccount.google.com/apppasswords

Avoid storing plaintext passwords in your scripts. Use environment variables or .env files in production environments.
