# Flowchart – Property Booking Process (Airbnb Clone)

This document explains the step-by-step flow of the **Property Booking** process in the Airbnb Clone backend system.

---

## 🎯 Objective
To visualize the logical sequence of how a property is booked by a guest — from checking availability to confirming payment and saving booking details.

---

## 🧠 Process Description

### 1. Start
The process begins when a **guest** chooses a property and requests to book specific dates.

### 2. Check Property Availability
The backend verifies if the selected property is available during the requested date range.

- If **not available** → return a “Booking Unavailable” response.  
- If **available** → proceed to booking creation.

### 3. Create Booking Record
The system creates a new booking entry with status **pending** in the database.

### 4. Process Payment
The system sends the payment details to the external **Payment Gateway (e.g., Stripe/PayPal)**.

- If payment **fails** → cancel the pending booking and notify the user.  
- If payment **succeeds** → update booking status to **confirmed**.

### 5. Send Confirmation
A confirmation message or email is sent to both the **guest** and **host**.

### 6. End
The process ends with a successful booking stored in the database.

---

## 📊 Diagram (to be added)
A flowchart will be added here showing the decision flow.  
File name: `booking-flow.png`
