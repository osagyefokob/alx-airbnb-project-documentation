# Use Case Diagram – Airbnb Clone Backend

This document explains the system interactions between users and the Airbnb Clone backend.

The **Use Case Diagram** visualizes how different types of users (actors) interact with the system and what core actions they can perform.  

---

## 🎭 Actors
1. **Guest**
   - Registers and logs into the system.
   - Searches and views properties.
   - Books available properties.
   - Makes payments.
   - Leaves reviews for properties.
   - Sends messages to hosts.

2. **Host**
   - Registers and logs into the system.
   - Creates, updates, and deletes property listings.
   - Views and manages bookings for their properties.
   - Sends and receives messages from guests.

3. **Admin**
   - Manages all users (guests and hosts).
   - Oversees properties, bookings, and payments.
   - Handles reports or flagged content.

4. **Payment Gateway (External Actor)**
   - Handles secure payment transactions for bookings.

---

## ⚙️ Use Cases
| Actor | Use Case |
|-------|-----------|
| Guest | Register/Login |
| Guest | Search & View Properties |
| Guest | Make Bookings |
| Guest | Make Payments |
| Guest | Leave Reviews |
| Guest | Send Messages |
| Host | Manage Properties |
| Host | View Bookings |
| Host | Send/Receive Messages |
| Admin | Manage Users |
| Admin | Manage Listings & Bookings |
| Payment Gateway | Process Payments |

---

## 🧩 Diagram (to be added later)
A visual Use Case Diagram will be added here once completed on Draw.io.  
File name: `use-case-diagram.png`

---

## 📘 Description
The Use Case Diagram provides a high-level view of how users interact with the backend system.  

- The **Guest** primarily interacts with the Booking, Payment, and Review features.  
- The **Host** interacts with Property Management and Messaging.  
- The **Admin** oversees and manages the entire system.  
- The **Payment Gateway** acts as an external service for transactions.
