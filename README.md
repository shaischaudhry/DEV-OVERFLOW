# DevOverflow - MERN Stack Overflow Clone

A full-featured Stack Overflow clone built with the **MERN stack** (MongoDB, Express.js, React, Node.js). This application demonstrates complete CRUD functionality, user authentication, real-time interactions, and modern web development practices.

## 🚀 Demo

Check out the `demo.mp4` file to see the application in action!

## 🛠️ Tech Stack

### Frontend
- **React 17** - Component-based UI library
- **Apollo Client** - State management and API communication
- **Material-UI** - Modern React component library
- **React Router** - Client-side routing
- **React Hook Form** - Form validation and handling

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **Apollo Server** - API server implementation
- **JWT** - JSON Web Token authentication

### Database
- **MongoDB** - NoSQL document database
- **Mongoose** - MongoDB object modeling

### Development Tools
- **Nodemon** - Development server auto-restart
- **ESLint** - Code linting and formatting
- **Bcrypt** - Password hashing

## ✨ Features

### Core Functionality
- **User Authentication** - Register, login, logout with JWT tokens
- **Question Management** - Create, read, update, delete questions
- **Answer System** - Post and manage answers to questions
- **Comment System** - Add comments to questions and answers
- **Voting System** - Upvote/downvote questions and answers
- **Tag System** - Categorize questions with multiple tags
- **Search & Filter** - Find questions by keywords and tags
- **User Profiles** - View user statistics and activity
- **Reputation System** - Track user reputation based on votes

### Advanced Features
- **Real-time Updates** - Dynamic content updates
- **Responsive Design** - Mobile-friendly interface
- **Pagination** - Efficient data loading
- **Sorting Options** - Sort by newest, oldest, most voted
- **Hot Algorithm** - Trending questions algorithm
- **Rich Text Support** - Formatted question and answer content

## 🏗️ Architecture

### API Endpoints

#### Data Retrieval
- Get paginated questions with filtering and sorting
- Get single question with answers and comments
- Get user profile and activity data
- Get all available tags with counts
- Get all users and top users by reputation

#### Data Operations
- User authentication (register/login)
- Question operations (create, edit, delete)
- Answer operations (create, edit, delete)
- Voting system for questions and answers
- Answer acceptance functionality
- Comment system for questions and answers

## 🗄️ Database Schema

### Collections
- **Users** - User profiles, authentication, reputation tracking
- **Questions** - Question content, metadata, voting, comments
- **Embedded Documents** - Answers and comments within questions

### Key Relationships
- Users → Questions (One-to-Many)
- Users → Answers (One-to-Many)
- Questions → Answers (One-to-Many)
- Questions/Answers → Comments (One-to-Many)
- Users ↔ Votes (Many-to-Many)

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### Installation

1. **Clone the repository**
```bash
git clone <repository-url>
cd WEBPROJECT
```

2. **Install dependencies**
```bash
# Install server dependencies
cd server
npm install

# Install client dependencies
cd ../client
npm install
```

3. **Environment Setup**
Create a `.env` file in the server directory:
```env
MONGODB_URI=mongodb://localhost:27017/techtalk-hub
PORT=4000
SECRET=your-jwt-secret-key
```

4. **Start MongoDB**
```bash
sudo systemctl start mongod
```

5. **Run the application**
```bash
# Start backend (from server directory)
npm run dev

# Start frontend (from client directory)
npm start
```

6. **Access the application**
- Frontend: http://localhost:3000
- Backend API: http://localhost:4000

## 📱 Usage

1. **Register/Login** - Create an account or login with existing credentials
2. **Browse Questions** - View questions sorted by various criteria
3. **Ask Questions** - Post new questions with relevant tags
4. **Provide Answers** - Help others by answering questions
5. **Vote & Comment** - Engage with the community through voting and commenting
6. **Build Reputation** - Gain reputation points through quality contributions

## 🔧 API Testing

The backend API is available at `http://localhost:4000` for testing and integration.

## 🤝 Contributing

This project demonstrates modern full-stack development practices including:
- Component-based architecture
- RESTful API design
- JWT authentication
- Database modeling
- Responsive UI/UX
- Error handling
- Code organization

## 📄 License

This project is for educational and demonstration purposes. 