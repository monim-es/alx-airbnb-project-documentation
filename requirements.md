# 📘 Airbnb Clone – Backend Requirements

This document outlines the technical and functional specifications for key backend features: **User Authentication**, **Property Management**, and **Booking System**.

---

## 🔐 1. User Authentication

### 🎯 Functional Requirements
- Users can register as **guests** or **hosts**.
- Users can log in using **email/password** or **OAuth** (Google, Facebook).
- Authenticated sessions managed via **JWT tokens**.

### 🔌 API Endpoints

#### `POST /api/auth/register`
Registers a new user.

**Input:**
```json
{
  "email": "user@example.com",
  "password": "SecurePass123",
  "role": "guest" | "host"
}
