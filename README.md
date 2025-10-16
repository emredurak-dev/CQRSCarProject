# 🚗 Car Project CQRS – Smart Car Rental Management System

## 📋 Overview
**Car Project CQRS** is a comprehensive **Car Rental Management System** built with **ASP.NET Core 9.0**, implementing the **CQRS (Command Query Responsibility Segregation)** pattern.  
It features an **AI-powered car recommendation engine**, **real-time API integrations**, and **modern UI/UX** designs for both customers and administrators.

---

## ✨ Key Features

### 🎯 User Experience
- **Smart Vehicle Search** – Filter by brand, fuel type, transmission, seating, price, and model year  
- **AI-Powered Recommendations** – Powered by **Groq AI API** for intelligent car suggestions  
- **Automatic Distance Calculation** – Real-time city-to-city calculations using a 25K+ dataset  
- **Live Fuel Prices** – Integrated **EIA API** with automatic TRY conversion  
- **Weather Information** – Real-time weather for better travel planning  
- **Modern Responsive UI** – Built using **Cental** and **Sneat** themes  

### 🔧 Admin Panel
- **Comprehensive Dashboard** – 15+ dynamic widgets with live stats  
- **AI Car Search Assistant** – AI integration for vehicle suggestions  
- **Advanced Filtering** – Multi-criteria search, sort, and pagination  
- **Live Integrations** – Fuel, weather, and exchange rates  
- **Full CRUD Management** – Vehicles, reservations, employees, and services  
- **Email Notifications** – Automatic mail system via **MailKit**

---

## 🏗️ Architecture & Tech Stack

### 🖥 Backend
- **Framework:** ASP.NET Core 9.0  
- **Pattern:** CQRS (Command Query Responsibility Segregation)  
- **ORM:** Entity Framework Core 9.0.8  
- **Database:** Microsoft SQL Server  
- **Email Service:** MailKit 4.13.0  

### 💻 Frontend
- **Framework:** Bootstrap 5.3.3  
- **Themes:** Cental (Main Site) + Sneat (Admin Panel)  
- **Icons:** Font Awesome 5.15.4, Bootstrap Icons  
- **Fonts:** Google Fonts (Lato, Montserrat)  
- **Scripts:** jQuery, Owl Carousel, Animate.css  

---

## 🗄 Database & Data Models
- **Approach:** Hybrid (Code First + Database First)  
- **Custom Dataset:** 25,000+ Turkish city-to-city distances  
- **Airport Data:** Full Turkish airport dataset  
- **Entity Configurations:** Optimized for performance and accuracy  

---

## 🌐 External API Integrations

### 1. **Groq AI API** – Car Recommendations
- **Endpoint:** `https://api.groq.com/openai/v1/chat/completions`  
- **Model:** `Llama-3.1-8b-instant`  
- **Purpose:** AI-based car recommendation engine  

### 2. **EIA API** – Fuel Prices
- **Endpoint:** `https://api.eia.gov/v2/petroleum/pri/gnd/data/`  
- **Purpose:** Fetches live fuel prices with TRY conversion  

### 3. **WeatherAPI** – Weather Data
- **Endpoint:** `http://api.weatherapi.com/v1/current.json`  
- **Purpose:** Provides live weather data (temperature, humidity, wind, conditions)  

### 4. **ExchangeRate-API** – Currency Conversion
- **Endpoint:** `https://v6.exchangerate-api.com/v6/{api_key}/latest/USD`  
- **Purpose:** Real-time USD–TRY conversion for fuel cost calculations  

---

## 🧩 Core Entities
| Entity | Description |
|--------|--------------|
| **Cars** | Vehicle details including pricing, specs, and availability |
| **Reservations** | Booking system with pickup/drop-off management |
| **Employees** | Staff and role management |
| **Messages** | Customer message tracking |
| **Distances** | 25,000+ Turkish city-to-city distances |
| **TurkeyAirports** | Full Turkish airport data |
| **Features/Services** | Company service listings |
| **Testimonials** | Customer feedback and reviews |
| **Sliders** | Homepage carousel content |
| **About** | Company mission and info |

---

## 🧮 Dataset Details
- **Distance Dataset:** 25,000+ Turkish intercity records  
- **Airport Dataset:** Comprehensive Turkish airport data  
- **Source:** Custom-built datasets for accuracy  
- **Update Cycle:** Periodically refreshed static data  

---

## 🎨 User Interface

### 🌍 Main Website (Cental Theme)
- **Responsive Design:** Mobile-first layout with Bootstrap 5  
- **Dynamic Carousel:** For featured cars and offers  
- **Interactive Components:**  
  - Vehicle filters  
  - Date-based booking forms  
  - AJAX contact form  
  - Testimonial slider  
  - Team showcase  
- **Color Palette:** Primary `#EA001E`, Secondary `#1F2E4E`  
- **Fonts:** Lato & Montserrat  

### ⚙️ Admin Panel (Sneat Theme)
- **Dashboard Widgets:**  
  - Vehicle count  
  - Active reservations  
  - Employee analytics  
  - Dataset statistics  
  - Live fuel prices  
  - Weather overview  
- **AI Integration:** Smart vehicle suggestion assistant  
- **Advanced Filtering:** Multi-criteria sorting and searching  
- **Data Visualization:** Charts and graphs for insights  

---

## 🔧 Configuration Guide

### 🗝 API Keys
1. **Groq AI API:** [https://console.groq.com/](https://console.groq.com/)  
2. **EIA API:** [https://www.eia.gov/opendata/](https://www.eia.gov/opendata/)  
3. **WeatherAPI:** [https://www.weatherapi.com/](https://www.weatherapi.com/)  
4. **ExchangeRate-API:** [https://www.exchangerate-api.com/](https://www.exchangerate-api.com/)

### 📧 Email Setup
- Configure SMTP credentials in `appsettings.json`  
- Use **Gmail App Password** for authentication  
- Enable **2FA** in your Gmail account  

---

## 📱 Functional Highlights

### 🚘 Vehicle Search & Booking
- Advanced filtering (brand, model, fuel, transmission, seats, price, year)  
- Sorting options (price, year, rating, brand)  
- AI-powered recommendations  
- Real-time availability checks  
- Automatic distance calculations  

### 🧭 Admin Management
- Real-time dashboard analytics  
- Vehicle CRUD operations  
- Full reservation lifecycle management  
- Employee and role management  
- Customer message handling  
- Service management  

### 🔗 Data Integration
- Live fuel price updates  
- Real-time weather and currency exchange data  
- Comprehensive distance dataset  

---

## 🛠️ Development Details

### ⚙️ CQRS Implementation
- **Commands:** Create, Update, Delete actions  
- **Queries:** Optimized data retrieval  
- **Handlers:** Independent command and query handlers  

### 🧩 Code Organization
- **Entities:** Domain models  
- **DbContext:** Entity Framework Core context  
- **Controllers:** MVC pattern for presentation  
- **Services:** Business logic & external API integration  
- **ViewComponents:** Modular UI components  
- **Models:** DTOs and ViewModels  

---

## 📸 Screenshots
![WhatsApp Image 2025-10-16 at 06 27 26_c7be63ac](https://github.com/user-attachments/assets/a47b6732-614a-4447-9bcc-57c384264ac2)
![WhatsApp Image 2025-10-16 at 06 27 26_233ef2e0](https://github.com/user-attachments/assets/28c9a5ac-b7c7-4fb7-9c5b-591558e5beac)
![WhatsApp Image 2025-10-16 at 06 27 25_76242980](https://github.com/user-attachments/assets/9d1d63a7-9361-4add-96c2-c6ff7bd02a77)
<img width="1900" height="1007" alt="Screenshot 2025-10-11 045719" src="https://github.com/user-attachments/assets/43cf29e6-6aa0-41d5-9210-ba7a532d2c6f" />
<img width="1900" height="862" alt="Screenshot 2025-10-11 045645" src="https://github.com/user-attachments/assets/054395d2-e61a-46d8-b265-08da13934587" />
<img width="1901" height="976" alt="Screenshot 2025-10-11 045621" src="https://github.com/user-attachments/assets/de6d3f81-580e-4856-add7-73952518542a" />
<img width="1901" height="935" alt="Screenshot 2025-10-11 045610" src="https://github.com/user-attachments/assets/5c09e0b6-48da-467e-bca7-0291209cdd79" />
<img width="1896" height="1007" alt="Screenshot 2025-10-11 045549" src="https://github.com/user-attachments/assets/0d09fdca-b485-4482-9a52-d69f40ef8175" />
