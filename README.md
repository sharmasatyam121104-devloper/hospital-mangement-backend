# Prescripto  
**Smart Hospital Management & Online Appointment Booking System**

Backend server for **Prescripto**, powering all three panels: **Admin**, **Doctor**, and **User**. It handles authentication, user & doctor management, appointment booking, and payment integrations.

---

## **Features**

### **Admin Panel**
- Add, edit, and manage **Doctors** and **Users**.  
- View all **appointments** and payment history.  
- Manage system-wide configurations and analytics.  

### **Doctor Panel**
- View and manage **appointments**.  
- Set available **time slots** for booking.  
- Track patient details and appointment status.  

### **User Panel**
- Browse and choose **Doctors**.  
- Book **appointments** for preferred time slots.  
- Make payments via **Razorpay** or **Stripe**.  
- View past and upcoming appointments.  

---

## **Technologies / Stack**

- Node.js  
- Express.js  
- MongoDB (Mongoose)  
- JWT (Authentication & Authorization)  
- Cloudinary (File Uploads)  
- Razorpay & Stripe (Payment Integration)  

---

## **Installation Steps**

1. Clone the repository:

```bash
git clone https://github.com/sharmasatyam121104-devloper/hospital-mangement-backend.git
cd hospital-mangement-backend
Install dependencies:


npm install
Create a .env file and add environment variables:

env

CURRENCY = "INR"
JWT_SECRET = ""

# Admin Panel Credentials
ADMIN_EMAIL = ""
ADMIN_PASSWORD = ""

# MongoDB Setup (required)
MONGODB_URI = ""

# Cloudinary Setup (required)
CLOUDINARY_NAME = ""
CLOUDINARY_API_KEY = ""
CLOUDINARY_SECRET_KEY = ""

# Razorpay Payment Integration
RAZORPAY_KEY_ID = ""
RAZORPAY_KEY_SECRET = ""

# Stripe Payment Integration
STRIPE_SECRET_KEY = ""
Start the server:

npm run server
Server will run on http://localhost:5000 (or the port specified in .env).

API Endpoints
Admin
/api/admin/login – Admin login

/api/admin/doctors – Add/Edit/Delete doctors

/api/admin/users – Manage users

/api/admin/appointments – View all appointments

Doctor
/api/doctor/login – Doctor login

/api/doctor/appointments – Manage own appointments

/api/doctor/timeslots – Set available time slots

User
/api/users/register – User signup

/api/users/login – User login

/api/appointments – Book and view appointments

/api/payments – Make payments via Razorpay or Stripe

Contributors / Author
Satyam Sharma

