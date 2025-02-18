# 🍔 Food Ordering MERN Application

A full-stack food ordering application built with the **MERN stack** (MongoDB, Express.js, React, Node.js). This project allows users to browse restaurants, place orders, and manage their profiles, while restaurant owners can manage their menus and orders.

## 🌟 Features

### **User Features**

The **Food Ordering MERN Application** is a full-stack web application that allows users to:

1. **Browse Restaurants:** Users can view a list of restaurants and their menus.
2. **Place Orders:** Users can add items to their cart and place orders.
3. **Track Orders:** Users can view their order history and track the status of their orders.
4. **Manage Profiles:** Users can update their profile information.

### **Restaurant Owner Features**

Restaurant owners can:

1. **Manage Menus:** Add, update, or delete menu items.
2. **View Orders:** See incoming orders and manage them.

### **General Features**

- Responsive design for mobile and desktop.
- Secure payment integration with **Stripe**.
- Real-time order updates.
- Image upload and management using **Cloudinary**.

## 🖥️ How the Website Works

1. **User Authentication:**

   - Users can sign up or log in using **Auth0**, which provides secure authentication.
   - Once logged in, users can access their profile and order history.

2. **Browsing Restaurants:**

   - Users can view a list of restaurants and their menus.
   - Each restaurant displays its menu items, prices, and images (stored in **Cloudinary**).

3. **Placing Orders:**

   - Users can add items to their cart and proceed to checkout.
   - The order is sent to the backend, where it is stored in the database.

4. **Order Management:**

   - Restaurant owners can view incoming orders and update their status (e.g., preparing, delivered).
   - Users can track the status of their orders in real-time.

5. **Image Management:**

   - Restaurant owners can upload images for menu items using **Cloudinary**.
   - Images are stored securely and displayed dynamically on the frontend.

## 🛠️ Technologies Used

### **Frontend**

- **React**: Frontend library for building user interfaces.
- **Vite**: Fast build tool for modern web applications.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **Shadcn UI**: Pre-built UI components for React.
- **React Router**: For client-side routing.
- **Axios**: For making HTTP requests to the backend.
- **React Query**: For managing server state and caching.
- **Zod**: For schema validation and type-safe forms.
- **Auth0**: For secure user authentication and authorization.

### **Backend**

- **Node.js**: JavaScript runtime for the server.
- **Express.js**: Web framework for building RESTful APIs.
- **MongoDB**: NoSQL database for storing application data.
- **Mongoose**: MongoDB object modeling for Node.js.
- **JWT (JSON Web Tokens)**: For user authentication and authorization.
- **Cloudinary**: For image upload and management.
- **Multer**: For handling file uploads.
- **Stripe**: For payment processing.

### **Other Tools**

- **Postman**: For testing API endpoints.
- **Git**: For version control.
- **Render**: For deployment.

## 📄 API Documentation

### Endpoints

- **Auth**

  - `POST /api/auth/login`: User login.
  - `POST /api/auth/register`: User registration.

- **Restaurants**

  - `GET /api/restaurants`: Get all restaurants.
  - `GET /api/restaurants/:id`: Get a specific restaurant.
  - `POST /api/restaurants`: Create a new restaurant.

- **Orders**

  - `POST /api/orders`: Place a new order.
  - `GET /api/orders/:id`: Get a specific order.
  - `GET /api/orders/user/:userId`: Get orders for a specific user.

- **Users**

  - `GET /api/users/:id`: Get user details.
  - `PUT /api/users/:id`: Update user details.
