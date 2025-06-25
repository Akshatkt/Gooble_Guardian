# Gooble Guardian

[Live Demo](https://gooble-guardian.onrender.com)

## Overview

Gooble Guardian is a comprehensive, user-friendly **central mess management system** designed to streamline the operations of cafeterias and messes, particularly those serving large groups such as hostels, colleges, or institutional settings. The platform simplifies everything from meal planning and ordering to inventory and payment management, ensuring a smooth experience for customers, cadets, and managers.

---

## Table of Contents

- [Features](#features)
- [Our Story](#our-story)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Scripts](#scripts)
- [Tech Stack](#tech-stack)
- [FAQs](#faqs)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- **Role-based Access**: Separate dashboards and permissions for Customers, Cadets, and Managers.
- **Centralized Inventory Management**: Managers can upgrade or degrade inventory, and everyone can view inventory levels.
- **User Management**: Managers can add or remove users, and users can edit their profiles and change passwords.
- **Payment Handling**: Secure payment history management and graphical representation of payment data for managers.
- **Feedback System**: Customers can submit feedback; managers can view all feedback.
- **Meal Planning**: View daily menus and manage meal orders.
- **Security**: Implements secure authentication and privacy for all user transactions and data.
- **Customizability**: System can be configured to fit the unique needs of different organizations.

---

## Our Story

A group of ambitious college students, frustrated by the chaotic and inefficient mess management systems on their campus, decided to build a better solution. With dedication and countless hours, they created Gooble Guardian—a platform that revolutionizes mess and cafeteria management, now used across various campuses and institutions.

---

## Getting Started

### Prerequisites

- Node.js (v16+ recommended)
- MongoDB instance (local or Atlas)
- Optional: Nodemon for development

### Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/Akshatkt/Gooble_Guardian.git
    cd Gooble_Guardian
    ```

2. **Install dependencies**
    ```bash
    npm install
    ```

3. **Set up environment variables**

    Create a `.env` file in the root with the following (example):
    ```
    PORT=3000
    MONGODB_URI=mongodb://localhost:27017/gooble_guardian
    JWT_SECRET=your_secret_key
    MAIL_USER=your_email@example.com
    MAIL_PASS=your_email_password
    ```

4. **Run the application**
    ```bash
    npm start
    ```
    For development with auto-reload:
    ```bash
    npm run dev
    ```

5. Visit [http://localhost:3000](http://localhost:3000) or the [Live Demo](https://gooble-guardian.onrender.com).

---

## Project Structure

```
.
├── app.js                # Main Express app configuration
├── index.js              # Entry point
├── controllers/          # Request/response logic per role (auth, cadet, manager, customer)
├── middleware/           # Auth, error handling, and request middleware
├── models/               # Mongoose schemas for Users, Inventory, Payments, etc.
├── routes/               # Route definitions for different user roles
├── public/               # Static assets (CSS, images, JS)
├── views/                # EJS templates for all pages
├── test/                 # Test cases for core functionalities
├── package.json
└── .gitignore
```

---

## Scripts

- `npm start` — Start the server.
- `npm run dev` — Start the server with nodemon for hot reloading.
- `npm test` — Run Mocha test suite.

---

## Tech Stack

- **Backend**: Node.js, Express.js
- **Frontend**: EJS templating, HTML, CSS, Bootstrap
- **Database**: MongoDB (via Mongoose)
- **Authentication**: JWT, bcrypt
- **Utilities**: Nodemailer (email), Method-Override, Morgan (logging)
- **Testing**: Mocha, Chai

---

## FAQs

### What is a central mess management system?
A central mess management system is a software solution that manages and streamlines the operations of a mess or cafeteria. It helps in managing customers, menus, payments, inventory, and other related tasks.

### Who can use Gooble Guardian?
Customers, cadets, and managers can each have different roles and access levels in the system.

### How to start using the service as a customer?
Sign up on the website, verify your account, and make a payment to the manager. Once processed, you’ll have access to the full platform.

---

## Contributing

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

---

## Contact

For support or suggestions, please file an issue or contact the maintainer via GitHub.

---

> _Gooble Guardian: Streamlining mess management for a happier, healthier community!_
