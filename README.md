# Portfolio Backend (Node.js & Express)

This is the backend server for my personal portfolio website, responsible for handling contact form submissions. It uses a secure API endpoint to receive messages and sends them directly to my email address.

## 🚀 Features

* **Contact Form API:** A RESTful API endpoint to securely receive and process contact form data from the frontend.
* **Email Service:** Uses Nodemailer to send messages from the contact form to my personal email.
* **Security:** Protects sensitive information (like email credentials) using environment variables (`.env`).
* **CORS Enabled:** Allows for secure communication between the frontend and this backend server.

---

## 🛠️ Tech Stack

* **Node.js:** The JavaScript runtime environment.
* **Express.js:** A minimal and flexible Node.js web application framework.
* **Nodemailer:** A module for sending emails via SMTP.
* **CORS:** Node.js middleware for handling cross-origin requests.
* **dotenv:** A module to load environment variables from a `.env` file.

---

## ⚙️ Setup and Installation

### Prerequisites

* Node.js (LTS version recommended)
* npm (comes with Node.js)

### Local Development

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Chengal-37/My-Portfolio-Backend.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd My-Portfolio-Backend
    ```
3.  **Install dependencies:**
    ```bash
    npm install
    ```
4.  **Create a `.env` file:**
    Create a file named `.env` in the root of the project and add your email credentials. **This file should not be committed to Git.**
    ```ini
    EMAIL_USER=your_email@gmail.com
    EMAIL_PASS=your_app_password
    ```
    *(Note: For Gmail, use a generated App Password, not your regular password.)*

5.  **Start the server:**
    ```bash
    node server.js
    ```
    The server will run on `http://localhost:5000`.

---

## 🔗 API Endpoint

**POST** `/api/contact`
* **Content-Type:** `application/json`
* **Body:**
    ```json
    {
      "name": "Your Name",
      "email": "your.email@example.com",
      "message": "Your message here."
    }
    ```

---

## 🌐 Live URL

This backend is deployed and available at:
**[https://my-portfolio-backend-zu90.onrender.com]**

---

## ©️ License

This project is open-source and available under the [MIT License]https://github.com/Chengal-37/My-Portfolio-Backend/blob/main/LICENSE.
