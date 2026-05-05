🚀 Task Management System

A modern full-stack application designed to manage tasks efficiently. Built using a combination of React on the frontend and Node.js with Express on the backend, along with MongoDB for data storage. The app enables users to collaborate, assign tasks, and track progress seamlessly.

✨ Key Highlights
🔐 Secure user authentication (signup & login)
👥 Manage teams and members easily
📝 Perform full task operations (create, edit, delete)
📅 Set deadlines and monitor task progress
👤 Access control based on user roles (Admin / User)
⚡ Smooth and user-friendly interface
🔔 Instant notifications for user actions
📱 Optimized for both mobile and desktop screens
🛠️ Technologies Used
Frontend
React (powered by Vite)
Tailwind CSS for styling
Axios for API communication
React Router for navigation
React Hot Toast for alerts
Lucide Icons
Backend
Node.js runtime
Express framework
MongoDB with Mongoose ODM
JWT for authentication
bcrypt for password encryption
📁 Folder Layout
root-directory/
├── client/        # Frontend source
│   ├── src/
│   ├── components/
│   ├── pages/
│   ├── custom-hooks/
│   └── App.jsx
│
├── server/        # Backend source
│   ├── models/
│   ├── routes/
│   ├── controllers/
│   ├── middleware/
│   └── index.js
🚀 Getting Started
1️⃣ Clone the repository
git clone https://github.com/your-username/task-manager.git
cd task-manager
2️⃣ Install dependencies

Frontend setup

cd client
npm install

Backend setup

cd server
npm install
3️⃣ Environment Configuration

Create .env files for both client and server.

Server (.env)

PORT=5000
MONGO_URI=your_database_url
JWT_SECRET=your_secret_key

Client (.env)

VITE_API_URL=http://localhost:5000/api
4️⃣ Run the Application

Start backend

cd server
npm run dev

Start frontend

cd client
npm run dev
🔐 Authentication Overview
Users can register or log in
A JWT token is generated upon authentication
The token is stored on the client side
Each request includes the token in headers for verification
Protected routes are accessible only to authorized users
📡 API Overview
Authentication Routes
Method	Endpoint
POST	/api/auth/register
POST	/api/auth/login
Task Routes
Method	Endpoint
GET	/api/tasks
POST	/api/tasks
PUT	/api/tasks/:taskId
DELETE	/api/tasks/:taskId
Project Routes
Method	Endpoint
GET	/api/projects
POST	/api/projects
