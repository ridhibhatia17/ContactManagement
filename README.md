# INGLU Contacts (Contact Management System)

A full-stack Contact Management web application built with the MERN stack (MongoDB, Express, React, Node.js). It provides a secure platform to manage personal and professional contacts with features like user authentication, Google OAuth integration, and complete CRUD functionality for contacts.

## Live Demo
- **Frontend Live URL:** [https://contact-management-virid.vercel.app](https://contact-management-virid.vercel.app)
- **Backend API URL:** [https://contactmanagement-production-755c.up.railway.app/](https://contactmanagement-production-755c.up.railway.app/)

## Features
- **User Authentication:** Secure email/password login utilizing bcrypt for password hashing and JWT for session management.
- **Google OAuth 2.0:** One-click seamless login using your Google account via Passport.js.
- **Contact Management:** Complete functionality to Create, Read, Update, and Delete contacts.
- **Responsive Design:** A beautifully styled user interface built with React that looks great on all devices.
- **RESTful API:** A robust Node/Express backend serving a JSON REST API.

## Tech Stack
### Frontend
- **React.js (Vite)**
- **React Router DOM** for navigation
- **Axios** for API requests
- **Lucide React** for icons
- **React Phone Input 2** for formatting phone numbers

### Backend
- **Node.js** & **Express.js**
- **MongoDB** & **Mongoose** for data storage
- **Passport.js** for Google OAuth 2.0 authentication
- **JSON Web Tokens (JWT)** for securing APIs
- **bcryptjs** for secure password hashing
- **Express-Session** and **CORS**

## Installation & Setup

### Prerequisites
- Node.js (v14 or higher)
- MongoDB Database (Local instance or MongoDB Atlas)
- Google Cloud Console account (for Google OAuth credentials)

### 1. Clone the repository
```bash
git clone <repository-url>
cd "Contact Management"
```

### 2. Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the `backend` folder based on the `.env.example` file and configure your variables:
   ```env
   PORT=5000
   MONGO_URI=mongodb://127.0.0.1:27017/contact-management
   JWT_SECRET=your_jwt_secure_secret_here
   SESSION_SECRET=your_session_secure_secret_here
   GOOGLE_CLIENT_ID=your_google_client_id_here
   GOOGLE_CLIENT_SECRET=your_google_client_secret_here
   FRONTEND_URL=http://localhost:5173
   ```
4. Start the backend development server:
   ```bash
   npm start
   ```

### 3. Frontend Setup
1. Open a new terminal and navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the `frontend` folder based on the `.env.example` file to ensure the Vite proxy connects properly to the API:
   ```env
   VITE_API_URL=http://localhost:5000/api
   ```
4. Start the frontend development server:
   ```bash
   npm run dev
   ```

## Usage

Once both servers are running, access the application by navigating to the frontend URL (typically `http://localhost:5173`). 
You can either create a new account via standard email/password registration or use the Google OAuth login to dive right in and start managing your contacts!

## Deployment
- The **frontend** is deployed and hosted on Vercel.
- The **backend** API is deployed and hosted on Railway.
