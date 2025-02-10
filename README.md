# Subscription Tracker

Subscription tracking API built using Node.js and Express, with MongoDB as the database. The API allows managing users, authentication, and subscriptions.

## Features

-   **Authentication**: Routes for user registration, login, and logout.
-   **Users**: Routes to create, update, list, and delete users.
-   **Subscriptions**: Routes to manage subscriptions, including creation, updating, listing, and cancellation.
-   **Database**: Connection to MongoDB using Mongoose.
-   **Configuration**: Environment variables managed with dotenv.

## Getting Started

### Prerequisites

-   Node.js
-   MongoDB

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/usingSubscription-tracker.git
    ```
2. Navigate to the project directory:
    ```bash
    cd usingSubscription-tracker
    ```
3. Install dependencies:
    ```bash
    npm install
    ```

### Configuration

Create a `.env` file in the root directory and add the following environment variables:

```bash
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
```

To start the application in development mode:

```bash
npm run dev
```

To start the application in production mode:

```bash
npm start
```

### API Endpoints

Authentication

-   `POST /api/auth/register` - Register a new user
-   `POST /api/auth/login` - Login a user
-   `POST /api/auth/logout` - Logout a user

Users

-   `GET /api/users` - Get all users
-   `GET /api/users/:id` - Get a user by ID
-   `PUT /api/users/:id` - Update a user by ID
-   `DELETE /api/users/:id` - Delete a user by ID

Subscriptions

-   `GET /api/subscriptions` - Get all subscriptions
-   `GET /api/subscriptions/:id` - Get a subscription by ID
-   `POST /api/subscriptions` - Create a new subscription
-   `PUT /api/subscriptions/:id` - Update a subscription by ID
-   `DELETE /api/subscriptions/:id` - Cancel a subscription by ID

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.
