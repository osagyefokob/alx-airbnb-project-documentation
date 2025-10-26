# Backend Feature Requirements – Airbnb Clone

This document outlines the technical and functional requirements for three key backend features:  
**User Authentication**, **Property Management**, and **Booking System**.

Each section defines the purpose, API endpoints, data inputs and outputs, and validation rules to guide backend development.

---

## 1. User Authentication

### **Purpose**
Handle user registration, login, and role-based access control (guest, host, admin).

### **Functional Requirements**
- Users can register with first name, last name, email, and password.
- Passwords must be hashed before storage.
- Users can log in using valid credentials.
- JWT tokens will be used for authentication.
- Invalid login attempts return appropriate error messages.

### **API Endpoints**
| Method | Endpoint | Description |
|--------|-----------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Authenticate existing user |
| GET | `/api/users/me` | Get current user profile (authenticated) |

### **Input / Output Examples**
**Input (POST /api/auth/register):**
```json
{
  "first_name": "Kofi",
  "last_name": "Owusu",
  "email": "kofi@example.com",
  "password": "securePass123"
}
