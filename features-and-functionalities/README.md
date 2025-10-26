# Features and Functionalities – Airbnb Clone Backend

This document outlines all the core backend features and functionalities of the Airbnb Clone application.  
It serves as the foundation for backend development, showing what the system must support before any code is written.

---

## 1. User Management
- Register new users with secure password hashing.
- User login and authentication using JWT.
- Role management: **guest**, **host**, and **admin**.
- Profile update: change password, email, or phone number.
- Authorization: restrict access based on roles.

---

## 2. Property Management
- Hosts can **create**, **update**, or **delete** property listings.
- Properties include name, description, price per night, and location.
- Guests can browse and search for properties by city, price, or rating.
- Manage property availability (booked vs. available).
- Upload and manage property images (future upgrade).

---

## 3. Booking System
- Guests can book available properties for a chosen date range.
- Prevent double bookings (availability checks).
- Booking statuses: **pending**, **confirmed**, **canceled**.
- Hosts can view and approve/cancel bookings.
- Automatic price calculation based on stay duration.

---

## 4. Payment Processing
- Secure integration with Stripe or PayPal APIs.
- Record every payment linked to a booking.
- Store transaction details: amount, method, date, status.
- Handle refunds or cancellations (future extension).

---

## 5. Reviews and Ratings
- Guests can rate properties (1–5) and leave feedback.
- Hosts can view guest reviews for their properties.
- Aggregate ratings visible on property listings.

---

## 6. Messaging System
- Guests and hosts can message each other directly.
- Each message includes sender, receiver, content, and timestamp.
- Future improvement: real-time chat via WebSockets.

---

## 7. Admin Panel (Future Enhancement)
- Admins manage users, properties, bookings, and payments.
- Dashboard with key statistics.
- Role-based access control.

---

## 8. Security and Performance
- Password hashing (bcrypt).
- Input validation and request sanitization.
- API rate limiting and logging.
- Environment-based configuration using `.env`.

---

## 9. Notifications (Future)
- Email/SMS alerts for bookings, cancellations, and payments.
- Optional push notifications.

---

## Diagram
A visual diagram of these features will be added here.  
(*Export `features-overview.png` from Draw.io and upload it in this same folder.*)
