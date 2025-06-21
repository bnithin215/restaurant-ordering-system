# restaurant-ordering-system
🍽️ Restaurant Ordering System

An intuitive Vue.js + Express.js full-stack web application for restaurant ordering. Customers can browse menus and place orders, while staff can manage menu items, orders, and more.
🚀 Features

    Customer-side

        Browse food & drink menu, grouped by categories

        Add items to cart, adjust quantities, remove items

        Place orders with automatic subtotal calculations

    Admin/Staff-side

        Manage menu items (create, edit, delete)

        View active orders by status (e.g. new, preparing, completed)

        Update order statuses and mark payments as completed

    Auth & User Management

        Customer registration, login, and profile management

        Staff/admin authentication for backend access

    Database

        MySQL (or your chosen SQL database), with support for migrations/schema

        Models for users, menu items, orders, order details

📦 Tech Stack

    Frontend: Vue.js, Vue Router, Vuex (state management)

    Backend: Node.js, Express.js, RESTful API

    Database: MySQL (via Sequelize or other ORM), with SQL scripts or migrations

    Other: Axios/fetch for API calls, dotenv for environment management

⚙️ Prerequisites

    Node.js ≥ 14

    MySQL (or compatible DB)

    Yarn or npm for package management

🛠️ Setup Instructions
1. Clone the repo

git clone https://github.com/bnithin215/restaurant-ordering-system.git
cd restaurant-ordering-system

2. Backend Setup

cd backend
cp .env.example .env
# Configure DB credentials, JWT secret, ports, etc.
npm install
# Initialize DB (e.g. run SQL scripts or migrations)
npm run migrate
npm start       # or `nodemon index.js` for live reload

3. Frontend Setup

cd ../frontend
cp .env.example .env
# Set VITE_API_URL to your backend endpoint
npm install
npm run dev     # launches local dev server (e.g. http://localhost:3000)

4. Usage

    Visit http://localhost:3000 to access the customer interface.

    Log in as staff (/admin or direct via API) to manage menu/orders.

    Place test orders to see full end-to-end workflow.
