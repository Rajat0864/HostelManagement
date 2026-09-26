# Hostel Management System

A full-stack hostel management web application built with React, Redux, Express, and MongoDB. It helps manage student and staff records, daily attendance, and hostel reporting with a simple administrative workflow.

## Overview

This project is designed to support day-to-day hostel administration. It includes:

- Student registration and profile management
- Daily attendance tracking
- Admin user management
- Attendance analysis and report generation
- CSV export for attendance data
- Cleanup of old attendance records by date range

## Tech Stack

### Frontend
- React
- Vite
- Redux and Redux Thunk
- React Router
- React Bootstrap
- Axios

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- bcryptjs

## Features

- User registration and login
- Admin-only access to management features
- Student CRUD operations
- Student detail and profile views
- Attendance marking for hostel residents
- Attendance summary and analysis screens
- CSV export for attendance records
- Deletion of old attendance entries based on number of days

## Project Structure

```text
Hostel-Management/
├── frontend/                 # React + Vite client app
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
├── server/                   # Express API server
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   └── index.js
├── package.json              # Root scripts
├── Procfile
├── README.md
└── .env                     # Local environment file
```

## Prerequisites

Make sure the following are installed:

- Node.js 20+
- npm
- MongoDB running locally or remotely

## Environment Variables

Create a `.env` file in the project root with:

```env
NODE_ENV=development
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/hostel_management
JWT_SECRET=your_strong_secret_key_here
```

## Installation

From the project root, run:

```bash
npm install
npm install --prefix frontend
```

## Running the app

### Development mode

```bash
npm run dev
```

This starts both services:

- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

### Backend only

```bash
npm run server
```

### Frontend only

```bash
npm run client
```

## Production build

Build the frontend:

```bash
npm run build --prefix frontend
```

Then start the server in production mode:

```bash
NODE_ENV=production npm start
```

In production, the Express server serves the built frontend from `frontend/dist`.

## API Overview

The backend includes routes for:

- User authentication
- Student management
- Attendance tracking
- Admin operations

## Contributing

Contributions are welcome. For major changes, please open an issue first to discuss the proposal.

## Notes

This application is intended for managing hostel operations, including daily attendance records, student profiles, and administrative reporting.
