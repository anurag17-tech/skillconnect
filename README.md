# Skill Share Platform

A web application that allows users to share their skills and connect with others who have similar skills. The platform is restricted to MITAOE students (email domain: @mitaoe.ac.in) and includes real-time chat functionality.

## Features

- User authentication with MITAOE email restriction
- Skill-based user matching
- Real-time chat functionality
- Profile management
- Skill search and filtering

## Prerequisites

- Node.js (v14 or higher)
- MongoDB
- npm or yarn

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd skill-share-platform
```

2. Install backend dependencies:
```bash
npm install
```

3. Install frontend dependencies:
```bash
cd client
npm install
```

4. Create a `.env` file in the root directory with the following variables:
```
MONGODB_URI=mongodb://localhost:27017/skill-share
JWT_SECRET=your-secret-key
PORT=5000
```

## Running the Application

1. Start the backend server:
```bash
npm run dev
```

2. In a new terminal, start the frontend development server:
```bash
cd client
npm start
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend: http://localhost:5000

## API Endpoints

### Authentication
- POST /api/auth/register - Register a new user
- POST /api/auth/login - Login user

### Users
- GET /api/users/profile - Get user profile
- PATCH /api/users/profile - Update user profile
- GET /api/users/match - Get users with matching skills
- GET /api/users/search - Search users by skill

### Chat
- GET /api/chat/:userId - Get or create chat with user
- GET /api/chat - Get all chats
- POST /api/chat/:chatId/messages - Add message to chat

## Technologies Used

### Backend
- Node.js
- Express.js
- MongoDB
- Socket.IO
- JWT Authentication

### Frontend
- React
- Material-UI
- Socket.IO Client
- React Router
- Axios

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 