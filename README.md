# Job Application Form – Django Project

This is a simple Django-based web application that allows users to submit a **job application form**.  
Once the form is submitted, the system **stores the applicant’s data in the database** and sends a **confirmation email** to the applicant.

---

## 🚀 Features

- 📝 Job Application Form (First Name, Last Name, Email, Start Date, Occupation)
- 📧 Sends automatic **confirmation email** to the user
- 💾 Stores all submitted applications in the database
- 🛠 Admin Panel to view all submitted forms
- 🎨 Clean frontend built using **Bootstrap 5**
- 📡 CSRF-protected POST form submission

---

## 📂 Project Structure

job_application_project/
│── job_application/ # App folder
│── templates/ # HTML templates
│── static/ # CSS/JS files (if used)
│── db.sqlite3 # Database
│── manage.py
└── README.md

## ✉️ Email Configuration

To enable email sending, add the following settings inside `settings.py`:

```python
EMAIL_BACKEND = "django.core.mail.backends.smtp.EmailBackend"
EMAIL_HOST = "smtp.gmail.com"
EMAIL_PORT = 587
EMAIL_USE_TLS = True
EMAIL_HOST_USER = "your_email@gmail.com"
EMAIL_HOST_PASSWORD = "your_app_password"
💡 Use a Gmail App Password — not your Gmail login password.


