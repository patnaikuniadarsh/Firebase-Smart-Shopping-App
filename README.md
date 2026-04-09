# 🛍️ Smart Shopping App - Firebase Based Dynamic Cart Management System

## Mobile Application Development Project

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Material Design](https://img.shields.io/badge/Material%20Design-757575?style=for-the-badge&logo=material-design&logoColor=white)

---

## 👑 Project Lead & Developer

| | |
|---|---|
| **👨‍💻 Name** | **P. Adarsh** |
| **Roll Number** | **A24126510152** |
| **Role** | **Team Leader & Full Stack Android Developer** |
| **Responsibilities** | Complete app architecture, Firebase integration, CartManager Singleton pattern, Dynamic button state implementation, Checkout & Order History logic, GitHub repository management |

---

## 👥 Team Members & Contributions

| Roll Number | Name | Role | Contributions |
|-------------|------|------|---------------|
| A24126510152 | **P. Adarsh** | **Team Leader & Developer** | **Full app development, Firebase integration, CartManager, Checkout, Order History, GitHub setup** |
| A24126510125 | Ch. Teja | UI/UX Designer | Designed XML layouts, Material Design implementation, Screenshot preparation |
| A24126510121 | A. Maneesh Chowdary | Documentation & Testing | Project documentation, Test cases, PPT presentation, Showcase preparation |

---

## 📌 Project Name

**Firebase-Based Smart Shopping Platform with Dynamic Cart Management**

## 📌 Overview
A modern Android e-commerce application with **real-time cloud synchronization**, **intelligent cart management using Singleton pattern**, and **personalized user experience**. Built with Java and Firebase.

## ✨ Key Features

| Feature | Description |
|---------|-------------|
| 🔐 Firebase Authentication | Secure email/password login with session email capture |
| 🛍️ Real-time Product Catalog | Live updates from Firebase Realtime Database |
| 🔍 Instant Search | TextWatcher filters products as user types |
| 🛒 Smart CartManager | Singleton pattern - prevents duplicate entries, increments quantities |
| ✅ Dynamic Button Feedback | "ADDED" button turns green when item is in cart |
| 📦 Validated Checkout | Phone & address required, name defaults to "Guest" |
| 📜 Personalized Order History | Client-side filtering shows only current user's orders |
| 🎨 Material Design UI | Blue (#2196F3) and Green (#4CAF50) theme |

## 🛠️ Technologies Used

| Category | Technology |
|----------|------------|
| Language | Java (JDK 17) |
| Framework | Android SDK |
| Database | Firebase Realtime Database |
| Authentication | Firebase Authentication |
| Design Pattern | Singleton (CartManager) |
| UI Components | RecyclerView, CardView, Material Components |
| Architecture | Model-View-Adapter (MVA) |

## 🗄️ Database Schema

### Products Node (Firebase Realtime Database)
```json
{
  "Products": {
    "productId": {
      "id": "prod_001",
      "name": "Wireless Headphones",
      "category": "Electronics",
      "description": "High quality wireless headphones",
      "imageEmoji": "🎧",
      "price": 1299.00
    }
  }
}

{
  "Orders": {
    "orderId": {
      "orderId": "-NxK2abc123",
      "userId": "user@email.com",
      "customerName": "Guest",
      "phone": "9876543210",
      "address": "123 Main Street, Vizag",
      "itemsSummary": "Headphones x1, Shoes x2",
      "totalAmount": 3597.00,
      "timestamp": "2026-04-09 14:35:22"
    }
  }
}

App Screens
Screen	Description
Splash Screen	App logo and branding with "Start Shopping" button
Login Screen	Email/password login, captures session email in CartManager
Signup Screen	New user registration via Firebase Authentication
Product Home Screen	Grid layout (2 columns) with real-time search, dynamic "ADDED" button
Cart Screen	List all items, quantities, grand total in pink
Checkout Screen	Name (optional, defaults to Guest), phone, address validation
Order History Screen	Past orders filtered by logged-in user email

**NAVIGATION FLOW**
SplashActivity → LoginActivity → SignupActivity (optional)
                ↓
        ProductHomeActivity
                ↓
           CartActivity
                ↓
         CheckoutActivity
                ↓
        OrderHistoryActivity
