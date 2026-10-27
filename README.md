# Savanna — E-Commerce Web Application

Savanna is a full-stack e-commerce web application inspired by the name of the African savanna. It is built with React, Node.js, Express, and MongoDB. Users can browse products, create an account, log in, and manage their shopping cart.

## Features

- Browse products with prices and descriptions
- Add products to the shopping cart
- Increase or decrease item quantities
- Remove items and clear the cart
- View the cart total
- User registration and login
- Password hashing and JWT-based authentication
- MongoDB database integration
- Responsive storefront UI

## Tech Stack

**Frontend**
- React
- Vite
- JavaScript
- CSS

**Backend**
- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Tokens (JWT)
- bcryptjs

## Project Structure

```text
savanna-e-commerce-app/
├── backend/
│   ├── models/
│   ├── routes/
│   ├── .gitignore
│   ├── dns.js
│   ├── seedProducts.js
│   ├── server.js
│   └── package.json
├── frontend/
│   ├── public/
│   ├── src/
│   └── package.json
└── README.md
```

## Getting Started

### Prerequisites

- Node.js and npm
- A MongoDB database, such as MongoDB Atlas
- Git

### 1. Get the project

Download or clone your Savanna repository, then open the project folder in your terminal.

### 2. Set up the backend

```bash
cd backend
npm install
```

Create a `.env` file inside the `backend` folder:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secure_secret_key
```

Replace the placeholder values with your own MongoDB connection string and a secure JWT secret. Never commit your `.env` file.

Start the backend:

```bash
npm run dev
```

### 3. Set up the frontend

Open a second terminal:

```bash
cd frontend
npm install
```

The frontend uses `http://localhost:5000` by default. If you need a different backend address, copy `.env.example` to `.env` and set `VITE_API_URL` to that address.

Start the frontend:

```bash
npm run dev
```

Open the local URL printed by Vite in your browser.

## Project Status

The core storefront, shopping cart, product API, and signup/login functionality are implemented. Configure your own environment variables and deployment services before publishing the app.

## Deployment

No deployment URLs are configured in this project copy. You can deploy the frontend, backend, and database using your own accounts and update this section with your live links.

## Security

- Environment variables are used for database credentials and the JWT secret.
- Passwords are hashed before storage.
- Authentication uses JSON Web Tokens.
- Sensitive configuration files are excluded from Git.

## Author

**Ayush Thakur**
