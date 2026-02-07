## 📌 API Overview

This project provides a complete set of RESTful APIs for an Airbnb-like booking platform, covering authentication, hotel and room management, inventory control, bookings, payments, and reporting.

---

## 🔐 User Authentication

- **POST** `/auth/signup` – User signup  
- **POST** `/auth/login` – User login  
- **POST** `/auth/refresh` – Refresh access token  

---

## 👤 User Profile & Guests

- **GET** `/users/profile` – Get my profile  
- **PATCH** `/users/profile` – Update my profile  
- **GET** `/users/myBookings` – Get my bookings  

**Guest Management**
- **GET** `/users/guests` – Get my guests  
- **POST** `/users/guests` – Add a guest  
- **PUT** `/users/guests/{guestId}` – Update a guest  
- **DELETE** `/users/guests/{guestId}` – Remove a guest  

---

## 🏨 Hotel Browsing

- **GET** `/hotels/search` – Search for hotels  
- **GET** `/hotels/{hotelId}/info` – Get hotel details  

---

## 🛠️ Admin – Hotel Management

- **POST** `/admin/hotels` – Create a hotel  
- **GET** `/admin/hotels` – Get all admin hotels  
- **GET** `/admin/hotels/{hotelId}` – Get hotel by ID  
- **PUT** `/admin/hotels/{hotelId}` – Update hotel details  
- **PATCH** `/admin/hotels/{hotelId}/activate` – Activate a hotel  
- **DELETE** `/admin/hotels/{hotelId}` – Delete a hotel  

---

## 🚪 Admin – Room Management

- **POST** `/admin/hotels/{hotelId}/rooms` – Create a room  
- **GET** `/admin/hotels/{hotelId}/rooms` – Retrieve all rooms  
- **GET** `/admin/hotels/{hotelId}/rooms/{roomId}` – Get room details  
- **PUT** `/admin/hotels/{hotelId}/rooms/{roomId}` – Update a room  
- **DELETE** `/admin/hotels/{hotelId}/rooms/{roomId}` – Delete a room  

---

## 📦 Admin – Inventory Management

- **GET** `/admin/inventory/rooms/{roomId}` – Retrieve inventory of a room  
- **PATCH** `/admin/inventory/rooms/{roomId}` – Update inventory for a room  

---

## 📅 Booking Flow

- **POST** `/bookings/init` – Initialize a new booking  
- **GET** `/bookings/{bookingId}/status` – Check booking status  
- **POST** `/bookings/{bookingId}/addGuests` – Add guests to a booking  
- **POST** `/bookings/{bookingId}/cancel` – Cancel a booking  

---

## 💳 Payments

- **POST** `/bookings/{bookingId}/payments` – Initiate payment  
- **POST** `/webhook/payment` – Capture payment (Webhook)

---

## 📊 Admin – Reports

- **GET** `/admin/hotels/{hotelId}/bookings` – Get all hotel bookings  
- **GET** `/admin/hotels/{hotelId}/reports` – Generate hotel booking report  

---

## 🗂️ Database Schema

### System Architecture & Entity Relationships

![System Flow](https://github.com/user-attachments/assets/e835a1af-bd39-403f-b3f8-1b996c1a5a86)

![Database Schema](https://github.com/user-attachments/assets/11a6b8e4-8de2-4c9e-93b1-7195969b6a03)
