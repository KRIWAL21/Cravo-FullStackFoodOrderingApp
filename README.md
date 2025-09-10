# Cravo - Full-Stack Food Ordering Platform (MernEats)

![MernEats application homepage](https://i.ibb.co/qj5qJg4/image-8ec7c5.png)

Welcome to **Cravo**, a complete, end-to-end food ordering web application built on the MERN stack. This platform serves as a two-sided marketplace, connecting customers with restaurants. Customers can search for local restaurants, browse menus, and place orders, while restaurant owners can sign up to manage their own digital storefront, including menus, orders, and restaurant details.

This project integrates modern web technologies to deliver a feature-rich, secure, and user-friendly experience, including authentication with Auth0, payment processing with Stripe, and image storage with Cloudinary.

---

## ## Key Features

#### **✅ For Customers:**
* **User Authentication:** Secure user registration and login handled by Auth0.
* **Restaurant Search:** Search for restaurants available in a specific city.
* **Advanced Filtering:** Filter search results by cuisine type (e.g., Pizza, Burgers, Vegan).
* **Sorting:** Sort restaurants by estimated delivery time or delivery price.
* **Menu Browsing:** View detailed restaurant information and menus.
* **Shopping Cart:** Add and remove items from a cart before checkout.
* **Secure Payments:** Integrated with the Stripe API for secure credit card processing.
* **Order History & Status:** View past orders and track the status of current orders.
* **User Profile:** Manage personal information, including address and city.

#### **✅ For Restaurant Owners:**
* **Restaurant Management:** Create and update restaurant details, including name, city, country, and delivery info.
* **Menu Management:** A full CRUD (Create, Read, Update, Delete) interface for menu items.
* **Image Uploads:** Upload a restaurant banner image using Cloudinary for cloud-based storage.
* **Order Management:** View a dashboard of incoming orders and update their status (e.g., "in progress", "out for delivery").

---

## ## Technology Stack

This project was built using the following technologies:

#### **🚀 Frontend:**
* **Framework:** React with TypeScript
* **Build Tool:** Vite
* **Styling:** Tailwind CSS & Shadcn/UI
* **Routing:** React Router
* **State Management:** React Query (TanStack Query)
* **Forms:** React Hook Form

#### **⚙️ Backend:**
* **Runtime:** Node.js
* **Framework:** Express.js
* **Database:** MongoDB
* **ODM:** Mongoose
* **Validation:** express-validator

#### **🌐 Services & APIs:**
* **Authentication:** Auth0
* **Payments:** Stripe
* **Image Storage:** Cloudinary

---

## ## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

You will need the following tools and accounts installed/created:
* Node.js & npm
* Git
* MongoDB Atlas Account
* Auth0 Account
* Cloudinary Account
* Stripe Account & Stripe CLI

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/KRIWAL21/Cravo-FullStackFoodOrderingApp.git](https://github.com/KRIWAL21/Cravo-FullStackFoodOrderingApp.git)
    cd Cravo-FullStackFoodOrderingApp
    ```

2.  **Setup the Backend:**
    ```bash
    cd Backend
    npm install
    cp .env.example .env
    ```
    * Fill in the required values in the newly created `.env` file (see below).

3.  **Setup the Frontend:**
    ```bash
    cd ../Frontend
    npm install
    cp .env.example .env
    ```
    * Fill in the required values in the newly created `.env` file (see below).

4.  **Run the Application:**
    * Run the backend and frontend servers in two separate terminals.
    * **Backend Terminal:**
        ```bash
        cd Backend
        npm run dev
        ```
    * **Frontend Terminal:**
        ```bash
        cd Frontend
        npm run dev
        ```
    * Open your browser and navigate to `http://localhost:5173`.

---

## ## Environment Variables

You will need to create `.env` files for both the backend and frontend and populate them with the following keys:

#### **`Backend/.env`**
```env
MONGODB_CONNECTION_STRING=
AUTH0_AUDIENCE=
AUTH0_ISSUER_BASE_URL=
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=
STRIPE_API_KEY=
STRIPE_WEBHOOK_SECRET=
FRONTEND_URL=http://localhost:5173
```

#### **`Frontend/.env`**
```env
VITE_API_BASE_URL=http://localhost:7000
VITE_AUTH0_DOMAIN=
VITE_AUTH0_CLIENT_ID=
VITE_AUTH0_AUDIENCE=
VITE_STRIPE_PUBLIC_KEY=
```

---

## ## Acknowledgments
* This project was built following the tutorial and guidance provided by **Chris Blakely**.
