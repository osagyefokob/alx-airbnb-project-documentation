# Data Flow Diagram (DFD) – Airbnb Clone Backend

This document explains how data flows through the Airbnb Clone backend system.  
It identifies the main entities, processes, data stores, and external actors that interact with the system.

---

## 🧠 Purpose
The DFD shows how data moves between users, backend processes, and the database for core features such as user authentication, property management, bookings, and payments.

---

## 🧩 Key Components

### **External Entities (Sources/Actors)**
- **Guest** – Provides input like registration details, search queries, and booking requests.
- **Host** – Provides property details, manages bookings.
- **Admin** – Oversees users and data integrity.
- **Payment Gateway** – Handles payment processing externally.

### **Processes**
1. **User Authentication Process**
   - Receives login/registration data.
   - Validates credentials and returns authentication token.
   - Stores user data securely in the database.

2. **Property Management Process**
   - Accepts property details from the host.
   - Stores or updates property data.
   - Returns confirmation to the host.

3. **Booking Process**
   - Accepts booking requests from guests.
   - Checks property availability.
   - Stores booking data and returns booking confirmation.

4. **Payment Process**
   - Sends payment details to the external gateway.
   - Receives confirmation or failure response.
   - Stores transaction record in the database.

5. **Review Process**
   - Accepts review data (rating, comment).
   - Stores review in the database.
   - Updates property rating.

---

### **Data Stores**
- **User Database** – Stores user profiles, credentials, and roles.
- **Property Database** – Stores property listings and details.
- **Booking Database** – Stores booking records and statuses.
- **Payment Database** – Stores payment information.
- **Review Database** – Stores ratings and comments.

---

## 📊 Diagram (to be added later)
A Data Flow Diagram (DFD) will be added here once completed on Draw.io.  
File name: `data-flow.png`

---

## 🧾 Description of Data Movement

| Actor | Input | Process | Data Store | Output |
|--------|--------|-----------|--------------|----------|
| Guest | Registration details | User Authentication | User DB | Account created |
| Host | Property info | Property Management | Property DB | Property saved |
| Guest | Booking request | Booking System | Booking DB | Booking confirmation |
| Guest | Payment details | Payment System | Payment DB | Payment receipt |
| Guest | Review data | Review System | Review DB | Review saved |
| Admin | Management actions | Admin Controls | All DBs | Reports, stats |

---

## 🧠 Summary
The DFD shows how each major backend process handles inputs, stores data, and returns responses.  
It ensures that data flow between components (users, backend, and databases) remains structured, secure, and efficient.
