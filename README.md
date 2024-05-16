# Stock Monitoring Project - Backend

Welcome to the Stock Monitoring Project backend repository! This document provides instructions for setting up and deploying the backend locally on your machine.

## Prerequisites

Make sure you have the following installed on your machine:

- [Node.js](https://nodejs.org/) (>= v14.x)
- [npm](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/)

## Installation

1. Clone the repository to your local machine:

    ```bash
    git clone <repository-url>
    ```

2. Navigate to the `backend` directory:

    ```bash
    cd backend
    ```

3. Install dependencies using npm or yarn:

    ```bash
    npm install
    # or
    yarn install
    ```

## Configuration

1. Create a `.env` file in the root of the `backend` directory.

2. Add the following environment variables to the `.env` file:

    ```plaintext
    JWT_SECRET=your_jwt_secret_here
    ```

    Replace `your_jwt_secret_here` with your desired JWT secret key.

## Database Setup

1. Ensure MongoDB is installed and running on your machine or use a cloud-based MongoDB service like MongoDB Atlas.

2. Configure the database connection string in `src/config/dbconfig.ts`:

    ```typescript
    const connectionString = `mongodb://<username>:<password>@<cluster-url>/<database-name>`;
    ```

    Replace `<username>`, `<password>`, `<cluster-url>`, and `<database-name>` with your MongoDB credentials and database details.

## Running the Server

### Production:

Run the following command to start the server in production mode:

```bash
npm start
# or
yarn start
