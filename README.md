# Portfolio Tracker - React Frontend

This is the frontend for the Portfolio Tracker application, built with React and Material UI. It interacts with the Flask backend to provide a user interface for managing financial portfolios and accessing educational content.

## Features

- User authentication (login, registration, profile management).
- Portfolio dashboard and detailed views.
- Management of assets within portfolios (add, update quantity, remove).
- Listing of educational courses and their materials.
- Responsive design for various screen sizes.
- Modern UI/UX with animations using Framer Motion and Material UI components.

## Project Structure

The project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

Key directories inside `src/`:
```
react_frontend/
├── public/                 # Static assets, index.html
├── src/
│   ├── animations/         # (Placeholder) Framer Motion variants, custom animations
│   ├── assets/             # Local static assets (images, fonts)
│   ├── components/         # Reusable UI components
│   │   └── layout/         # Main layout components (AppBar, Drawer, etc.)
│   ├── contexts/           # React Context API providers (e.g., AuthContext)
│   ├── hooks/              # Custom React hooks (e.g., useDebounce)
│   ├── pages/              # Top-level route components
│   ├── services/           # Modules for API calls (axios instances, specific service files)
│   ├── themes/             # Material UI theme customization (defaultTheme.js)
│   ├── utils/              # Utility functions
│   ├── App.js              # Main application component with routing
│   ├── index.js            # Entry point, renders App, applies ThemeProvider & AuthProvider
│   └── ...                 # Other standard CRA files
├── .env.example            # Example environment variables for frontend
└── package.json            # Project dependencies and scripts
```

## Setup and Installation

1.  **Clone the repository (if applicable).**

2.  **Navigate to the `react_frontend` directory:**
    ```bash
    cd react_frontend
    ```

3.  **Install dependencies:**
    Make sure you have Node.js and npm (or Yarn) installed.
    ```bash
    npm install
    # OR
    # yarn install
    ```

4.  **Set up environment variables:**
    Copy `.env.example` to a new file named `.env.development.local` or `.env.production.local` (or just `.env`). This file is gitignored by default by Create React App.
    Update the variables, especially:
    - `REACT_APP_API_BASE_URL`: The base URL for the Flask backend API (e.g., `http://localhost:5001/api`).

    Example `.env.development.local`:
    ```
    REACT_APP_API_BASE_URL=http://localhost:5001/api
    ```

## Available Scripts

In the project directory, you can run:

### `npm start` or `yarn start`

Runs the app in development mode.
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.
The page will reload when you make changes.
You may also see any lint errors in the console. The Flask backend should be running concurrently (e.g., on port 5001).

### `npm test` or `yarn test`

Launches the test runner in interactive watch mode.
(TODO: Set up Jest and React Testing Library tests).

### `npm run build` or `yarn build`

Builds the app for production to the `build` folder.
It correctly bundles React in production mode and optimizes the build for the best performance.
The build is minified and the filenames include hashes.

### `npm run eject` or `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**
If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

## Key Dependencies

- **React:** JavaScript library for building user interfaces.
- **React Router DOM:** For declarative routing.
- **Material UI (`@mui/material`):** Comprehensive UI component library.
- **Emotion (`@emotion/react`, `@emotion/styled`):** Styling engine for Material UI.
- **Framer Motion:** For animations and gestures.
- **Axios:** Promise-based HTTP client for API calls.
- **Prop Types:** Runtime type checking for React props.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).
To learn React, check out the [React documentation](https://reactjs.org/).
```
