E-commerce-Assignment
This is a full-stack e-commerce application built with React, Vite, Node.js, Express, and MongoDB. The project allows users to browse products, add them to the cart, and proceed with a checkout process. The backend handles user authentication, product management, and payment integration with Stripe.

Table of Contents
Tech Stack
Features
Installation
Frontend Configuration
Backend Configuration
Environment Variables
Running Locally
License
Tech Stack
Frontend: React, Vite, Tailwind CSS
Backend: Node.js, Express, MongoDB
Authentication: JWT (JSON Web Token)
Payment Integration: Stripe
Environment: .env for configuration
Packages:
Server:
bash
Copy code
npm install express dotenv mongoose jsonwebtoken stripe cloudinary cookie-parser bcrypt.js ioredis nodemon
Frontend:
bash
Copy code
npm install axios @stripe/stripe-js framer-motion lucide-react react-confetti react-hot-toast react-router-dom recharts zustand
Features
User Authentication: Sign up, login, and session management.
Product Management: Display products, product categories, and product details.
Shopping Cart: Add products to the cart, update quantities, and remove items.
Checkout: Integrated with Stripe for handling payments.
Responsive Design: Built with Tailwind CSS for mobile-first design.
Coupon System: Users can apply, remove, and validate discount coupons during checkout.
Installation
1. Clone the Git repository:
Open a terminal and run the following command to clone the repository:

bash
Copy code
git clone https://github.com/charindu24/FullStack_E-Commerce_Site24.git
2. Navigate into the project directory:
bash
Copy code
cd FullStack_E-Commerce_Site24
3. Install dependencies for both frontend and backend:
bash
Copy code
npm install
cd frontend
npm install
cd ..
4. Set up environment variables (see below).
Frontend Configuration
Navigate to the frontend directory and run the development server:
bash
Copy code
cd frontend
npm run dev
Backend Configuration
Navigate to the backend directory and run the development server:
bash
Copy code
cd backend
npm run dev
Example Backend .env file:
env
Copy code
MONGO_URI=mongodb+srv://your-mongo-uri
STRIPE_SECRET_KEY=your-stripe-secret-key
ACCESS_TOKEN_SECRET=your-access-token-secret
REFRESH_TOKEN_SECRET=your-refresh-token-secret
COUPON_SECRET_KEY=your-coupon-secret-key  # Secret key for coupon functionality
Running Locally
Install all dependencies by running npm install in the root and frontend directories.
Set up your MongoDB connection, Stripe keys, and Coupon secret in the .env files.
Start both the frontend and backend servers:
Frontend: npm run dev (inside the frontend folder)
Backend: npm run dev (inside the backend folder)
The frontend will be available at http://localhost:3000 and the backend at http://localhost:5000.

License
This project is licensed under the MIT License.
