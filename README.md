# 🛍️ Sales Savvy – E-Commerce Frontend Application

![React](https://img.shields.io/badge/React-19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS 4](https://img.shields.io/badge/Tailwind_CSS-4.0-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Container-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-Build-646CFF?style=for-the-badge&logo=vite&logoColor=white)

## 📖 Project Overview
**Sales Savvy** is a modern, full-stack e-commerce frontend built with **React 19** and **TypeScript**. It features a robust customer shopping experience and a comprehensive Admin Dashboard for business management. The application is styled with **Tailwind CSS 4** and **shadcn/ui**, ensuring a responsive and accessible design.

It is production-ready, supporting containerization via **Docker** and serving via **Nginx**.

---

## 🛠️ Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Core** | React 19, TypeScript, React Router |
| **Styling & UI** | Tailwind CSS 4, shadcn/ui |
| **State & Forms** | React Hook Form, Zod Validation |
| **Network** | Axios (API Requests) |
| **Payments** | Razorpay Integration |
| **Build Tooling** | Vite, pnpm |
| **DevOps** | Docker, Nginx (Production Serving) |

---

## 🚀 Features

### 🛒 Customer Features
* **User Authentication:** Secure Login and Registration flows.
* **Product Discovery:** Browse products by category with optimized navigation.
* **Smart Cart:** Full management (Add, Remove, Update quantities) with real-time calculations.
* **Secure Checkout:** Integrated **Razorpay** gateway for safe transactions.
* **Order Tracking:** View detailed order history.
* **Personalization:** Dark/Light theme toggle for user preference.

### 📊 Admin Dashboard
* **User Management:** View and edit user details and assign roles.
* **Product Management:** Full CRUD (Create, Read, Update, Delete) capabilities for inventory.
* **Business Analytics:** Interactive dashboard featuring:
    * 📈 Overall Business Summary
    * 📅 Yearly Revenue Reports
    * 📆 Monthly Performance Analysis
    * 📊 Daily Sales Reports
    * 🏷️ Category-wise Sales Breakdown

---

## ⚡ Getting Started

### Prerequisites
* **Node.js** (v24 or higher recommended)
* **pnpm** (installed globally: `npm install -g pnpm`)
* **Backend API** (Must be running locally or remotely)

### 📥 Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/AbhishekN843/SalesSavvy.git](https://github.com/AbhishekN843/SalesSavvy.git)
    cd SalesSavvy
    ```

2.  **Install dependencies:**
    ```bash
    pnpm install
    ```

3.  **Environment Setup:**
    Create a `.env` file in the root directory:
    ```bash
    cp .env.example .env
    ```
    Update the variables in `.env`:
    ```env
    VITE_APP_NAME=SalesSavvy
    VITE_API_URL=http://localhost:8080/api  # Update with your Backend URL
    VITE_RZP_KEY_ID=your_razorpay_key
    COMPOSE_PROJECT_NAME=salessavvy-frontend
    ```

---

## 🏃‍♂️ Development & Production

### Run Development Server
Start the Vite development server with hot-reload:
```bash
pnpm dev
```

The app will be available at http://localhost:5173


 **Production Build:**
Create an optimized build for production (Static Files):

```bash
pnpm build
```
Preview the production build locally:

```bash
pnpm preview
```

**🐳 Docker Deployment:**

This project includes full Docker support for containerized deployment (Nginx Server).

Build and run with Docker Compose:

```bash
docker compose up --build
```
The containerized app will be available at http://localhost:5173

Developed by Abhishek
