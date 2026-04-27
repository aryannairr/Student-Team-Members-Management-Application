# Student-Team-Members-Management-Application
A full-stack web application to manage student team members, allowing users to add, view, and explore member details with image upload support. Built with React, Node.js, Express, and MongoDB.
Tech Stack
Frontend: React.js, React Router, CSS
Backend: Node.js, Express.js
Database: MongoDB
Tools: Axios, Multer for file uploads
Installation Steps
Prerequisites
Node.js (v14 or higher)
npm or yarn
Backend Setup
Navigate to the backend directory:

cd backend
Install dependencies:

npm install
Start the backend server:

npm start
Or for development:

npm run dev
Note: Currently using in-memory storage for demo purposes. MongoDB integration will be added once the database is properly configured.

Frontend Setup
Navigate to the frontend directory:

cd frontend
Install dependencies:

npm install
Start the React development server:

npm start
The application will be available at http://localhost:3000

API Endpoints
Base URL: /api
POST /api/members

Add new member
Request: Form data with name, role, email, contact, additional_info, image
Response: { status: "success", member_id: "string" }
GET /api/members

Fetch all members
Response: Array of member objects [{ id, name, role, image }, ...]
GET /api/members/:id

Fetch single member details
Response: { id, name, role, email, contact, image, additional_info, created_at }
Run Instructions
Ensure MongoDB is running
Start backend server: cd backend && npm start
Start frontend: cd frontend && npm start
Open browser to http://localhost:3000
Features
Add team members with profile images
View all team members in card format
Detailed view of individual members
Responsive design
Form validation
Secure file uploads
Project Structure
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── routes/
│   │   └── App.js
├── backend/
│   ├── models/
│   ├── routes/
│   ├── controllers/
│   ├── uploads/
│   └── server.js
└── README.md
