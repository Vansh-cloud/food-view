# Food Reel Project

A full-stack food sharing application with React frontend and Node.js backend.

## Project Structure

```
food reel/
├── backend/          # Node.js/Express API server
├── frontend/         # React/Vite client application
└── videos/           # Video assets
```

## Setup Instructions

### Prerequisites
- Node.js (v16 or higher)
- MongoDB (local installation or MongoDB Atlas)
- npm or yarn

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd "food reel/backend"
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure environment variables:
   - The `.env` file is already configured with default values
   - Update `MONGO_URI` if using a different database
   - Update `JWT_SECRET` with a secure secret for production
   - Configure ImageKit credentials if using image uploads

4. Start the development server:
   ```bash
   npm run dev
   ```
   The backend will run on `http://localhost:3000`

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd "food reel/frontend"
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```
   The frontend will run on `http://localhost:5173`

### Running Both Services

To run both backend and frontend simultaneously:

1. Open two terminal windows
2. In the first terminal, start the backend server
3. In the second terminal, start the frontend server

## Features

- User authentication (regular users and food partners)
- Food reel/post creation and viewing
- User profiles and food partner profiles
- Save/like functionality
- Responsive design with theme toggle
- Image upload support with ImageKit integration

## API Endpoints

- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/partner/register` - Food partner registration
- `POST /api/auth/partner/login` - Food partner login
- Food and partner-specific routes available

## Issues Fixed

1. ✅ CSS import paths corrected (`auth.css` → `auth-shared.css`)
2. ✅ Missing Profile component created
3. ✅ Build configuration verified
4. ✅ Dependencies installed and verified
5. ✅ Environment configuration set up

## Technologies Used

### Frontend
- React 19
- React Router DOM 7
- Vite (with Rolldown)
- Axios for API calls
- CSS3 for styling

### Backend
- Node.js with Express
- MongoDB with Mongoose
- JWT for authentication
- bcrypt for password hashing
- ImageKit for image storage
- CORS configuration for cross-origin requests
