# 2YourDoor: The Next-Generation Food Delivery Platform

Welcome to the official repository for **2YourDoor**, a cutting-edge, full-stack food ordering application built with the powerful MERN (MongoDB, Express.js, React, Node.js) architecture. Our platform is engineered to deliver an intuitive, secure, and seamless experience for both customers and administrators.

## Core Functionality

- **Dual-Panel Architecture**: Separate, feature-rich interfaces for both end-users and administrators.
- **Secure User Authentication**: Robust user security implemented with JSON Web Tokens (JWT) and Bcrypt password hashing.
- **Integrated Payment Gateway**: Seamless and secure online payments powered by the Stripe API.
- **Comprehensive User Experience**: Full suite of user actions including registration, login/logout, cart management, and order placement.
- **Advanced Admin Controls**: Empowering administrators with complete control over product listings, order fulfillment, and user management.
- **Dynamic Food Filtering**: Users can easily find what they're looking for with our intuitive product filtering system.
- **Modern API Design**: Built on a foundation of RESTful APIs with role-based access control for enhanced security.
- **User-Friendly Notifications**: Engaging and informative alerts to keep users updated on their order status.

## Getting Started Locally

To get a local copy up and running, follow these simple steps.

### Prerequisites

- Node.js and npm installed on your machine.
- A MongoDB database instance (local or cloud-based).
- A Stripe account for payment processing.

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/codingwithshawnyt/2YourDoor.git](https://github.com/codingwithshawnyt/2YourDoor.git)
    cd Food-Delivery
    ```

2.  **Install Frontend Dependencies:**
    ```bash
    cd frontend
    npm install
    ```

3.  **Install Admin Panel Dependencies:**
    ```bash
    cd ../admin
    npm install
    ```

4.  **Install Backend Dependencies:**
    ```bash
    cd ../backend
    npm install
    ```

5.  **Configure Environment Variables:**
    Create a `.env` file in the `backend` directory and add the following variables:
    ```
    JWT_SECRET=YOUR_CUSTOM_JWT_SECRET
    SALT=YOUR_CUSTOM_SALT_VALUE
    MONGO_URL=YOUR_MONGODB_CONNECTION_STRING
    STRIPE_SECRET_KEY=YOUR_STRIPE_API_SECRET_KEY
    ```

6.  **Link Frontend, Admin, and Backend:**
    - In `admin/src/App.jsx`, set `const url = 'YOUR_BACKEND_URL';`
    - In `frontend/src/context/StoreContext.js`, set `const url = 'YOUR_BACKEND_URL';`
    - In `backend/controllers/orderController.js`, set `const frontend_url = 'YOUR_FRONTEND_URL';`

7.  **Launch the Application:**
    - **Start the Backend:**
      ```bash
      cd backend
      nodemon server.js
      ```
    - **Start the Frontend:**
      ```bash
      cd ../frontend
      npm start
      ```
    - **Start the Admin Panel:**
      ```bash
      cd ../admin
      npm start
      ```

## Technology Stack

This project is built using a modern and robust technology stack:

-   **Frontend:** [React](https://reactjs.org/)
-   **Backend:** [Node.js](https://nodejs.org/en), [Express.js](https://expressjs.com/)
-   **Database:** [MongoDB](https://www.mongodb.com/)
-   **Payments:** [Stripe](https://stripe.com/)
-   **Authentication:** [JWT (JSON Web Token)](https://jwt.io/introduction)
-   **File Uploads:** [Multer](https://www.npmjs.com/package/multer)

## Deployment

This application is deployed and hosted on [Render](https://render.com/).

## How to Contribute

We welcome and encourage contributions to the project! Please feel free to open a pull request to suggest changes or add new features.
