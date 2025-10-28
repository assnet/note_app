ℹ️ This was not showed in the tutorial
please add
in `notes_app_backend/.env`

```
PORT=3000
FRONTEND_URL=http://localhost:5173
```

and in `notes_app_react/.env`

```
VITE_FRONTEND_URL=http://localhost:5173
VITE_BACKEND_URL=http://localhost:3000
```

### Environment Variables

The application uses environment variables for configuration instead of hardcoded URLs. Create `.env` files in both backend and frontend directories as described in their respective setup sections.

# Scalable Notes App

This is a full-stack serverless note-taking application using React.js for the frontend and a Node.js backend powered by AWS services.

## Tech Stack

**Frontend:**

- React.js
- Vite
- Tailwind CSS
- daisyUI
- React Router
- oidc-client-ts

**Backend:**

- Node.js
- Express.js
- AWS SDK (Cognito, DynamoDB)

## Getting Started

### Prerequisites

- Node.js
- pnpm
- An AWS account with configured credentials (applied using aws cli)

### Backend Setup

1.  Navigate to the `notes_app_backend` directory:
    ```bash
    cd notes_app_backend
    ```
2.  Create a `.env` file with the following variables:
    ```env
    PORT=3000
    FRONTEND_URL=http://localhost:5173
    ```
3.  Install the dependencies:
    ```bash
    pnpm install
    ```
4.  Start the backend server:
    ```bash
    pnpm start
    ```

### Frontend Setup

1.  Navigate to the `notes_app_react` directory:
    ```bash
    cd notes_app_react
    ```
2.  Create a `.env` file with the following variables:
    ```env
    VITE_FRONTEND_URL=http://localhost:5173
    VITE_BACKEND_URL=http://localhost:3000
    ```
3.  Install the dependencies:
    ```bash
    pnpm install
    ```
4.  Start the frontend development server:
    ```bash
    pnpm dev
    ```

## Project Structure

```
.
├── notes_app_backend
│   ├── controllers
│   ├── middleware
│   ├── routes
│   ├── config
│   ├── index.js
│   └── package.json
└── notes_app_react
    ├── public
    ├── src
    │   ├── assets
    │   ├── components
    │   ├── App.jsx
    │   └── main.jsx
    ├── index.html
    └── package.json
```
