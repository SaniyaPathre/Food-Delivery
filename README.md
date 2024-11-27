# Food Delivery Web App

## Description
The Food Delivery Web App is an end-to-end platform where customers can view and order food from various restaurants. It supports user authentication, cart management, and payment processing. The application also features an admin panel where restaurant and order data can be managed efficiently.

## Key Features
- **User Authentication**: Secure registration and login using JWT tokens.
- **RBAC (Role-Based Access Control)**: Users are assigned roles (Admin, User, Moderator), ensuring restricted access to resources.
- **Admin Dashboard**: Admins can manage users, restaurants, and orders.
- **Order Processing**: Users can browse the menu, add items to the cart, and securely check out via Stripe.

## Role in RBAC Implementation
As part of the project, I implemented Role-Based Access Control (RBAC) to ensure the right level of access for different users. I used JWT-based authentication and defined roles with varying permissions:
- **Admin**: Full access to manage users, restaurants, and orders.
- **User**: Can browse restaurants, place orders, and update their profile.
- **Moderator**: Limited permissions to moderate content but not manage orders.

The RBAC system ensures a secure and structured access mechanism, enhancing both the user experience and data integrity.

## Tech Stack
- **Frontend**: ReactJS, Axios for API calls, React Router for navigation.
- **Backend**: Node.js, Express.js for API handling.
- **Database**: MongoDB (Mongoose ORM for database interactions).
- **Authentication**: JWT (JSON Web Tokens) for secure authentication.
- **Payment Integration**: Stripe for processing payments.

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/SaniyaPathre/Food-Delivery.git
   cd Food-Delivery
   ```
2. Install the required dependencies:
   - For backend:
     ```bash
     cd backend
     npm install
     ```
   - For frontend:
     ```bash
     cd frontend
     npm install
     ```
3. Set up your environment variables for JWT, MongoDB, and Stripe in `.env` files.
4. Run the backend server:
   ```bash
   npm run dev
   ```
5. Run the frontend application:
   ```bash
   npm run dev
   ```
##Conclusion
This project demonstrates how to implement a secure food delivery system with RBAC using the MERN stack. It incorporates role-specific permissions, ensuring that sensitive data and functionalities are only accessible to authorized users.
