# products-api-app
# E-Commerce API

This is a simple e-commerce API built using Node.js, Express, and MongoDB. It provides authentication, product management, and order processing functionalities.

## Features

- User registration and authentication (JWT-based)
- CRUD operations for products
- Order creation and retrieval
- Secure password hashing with bcrypt

## Technologies Used

- Node.js
- Express
- MongoDB & Mongoose
- JSON Web Tokens (JWT)
- bcrypt (for password hashing)
- dotenv (for environment variables)
- CORS

## Installation

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)

### Steps to Set Up

1. **Clone the repository:**

   ```sh
   git clone https://github.com/BlockyAit/products-api-app
   cd your-project-folder
   ```

2. **Install dependencies:**

   ```sh
   npm install
   ```

3. **Set up environment variables:**

   - Create a `.env` file in the root directory
   - Add the following variables:
     ```sh
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_secret_key
     PORT=5000 # Or any preferred port
     ```

4. **Start the server:**

   ```sh
   node product.js
   ```

   Or using nodemon for auto-restart during development:

   ```sh
   npx nodemon product.js
   ```

## API Endpoints

### Authentication

| Method | Endpoint    | Description         |
| ------ | ----------- | ------------------- |
| POST   | `/register` | Register a new user |
| POST   | `/login`    | User login (JWT)    |

### Products

| Method | Endpoint        | Description           |
| ------ | --------------- | --------------------- |
| POST   | `/products`     | Add a new product     |
| GET    | `/products`     | Retrieve all products |
| PUT    | `/products/:id` | Update a product      |
| DELETE | `/products/:id` | Delete a product      |

### Orders

| Method | Endpoint          | Description                |
| ------ | ----------------- | -------------------------- |
| POST   | `/orders`         | Create a new order         |
| GET    | `/orders/:userId` | Retrieve orders by user ID |
| DELETE | `/orders/:id`     | Delete an order            |

## Deployment

### Deploying to Render or Heroku

1. Push code to GitHub.
2. Connect GitHub repo to Render/Heroku.
3. Set environment variables in the cloud platform.
4. Deploy and get the live URL.

