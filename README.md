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

📧 How Email Sending Works
Inside your views.py, after the form is saved:

python
Copy code
from django.core.mail import send_mail

send_mail(
    subject="Job Application Received",
    message=f"Hello {first_name},\n\nThank you for applying! We received your application.",
    from_email="your_email@gmail.com",
    recipient_list=[email],
    fail_silently=False,
)
The user receives a confirmation email instantly after submitting the form.

🖼 Screenshots
(Add your form screenshot here)

👨‍💻 Admin Panel
Use Django admin to manage applications:

nginx
Copy code
python manage.py createsuperuser
Login at:

arduino
Copy code
http://127.0.0.1:8000/admin/
📜 License
This project is open-source and free to use.

🤝 Contributing
Pull requests are welcome.
For major changes, please open an issue first.

📞 Contact
For support or queries, contact:

makefile
Copy code
Developer: Aniket Kolekar
Email: your_email@gmail.com
yaml
Copy code

---

If you want, I can also create:

✅ A **professional GitHub README with badges**  
✅ A **project logo**  
✅ A **video demo section**  
✅ A **setup guide with screenshots**

Just tell me!











