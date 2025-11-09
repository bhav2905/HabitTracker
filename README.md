# 📚✨ All-in-One Habit & Exam Preparation Tracker

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/BhavAnsh/habit-exam-tracker?style=social)
![GitHub forks](https://img.shields.io/github/forks/BhavAnsh/habit-exam-tracker?style=social)
![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)
![Build](https://img.shields.io/badge/Build-Passing-success)
![Made with](https://img.shields.io/badge/Made%20with-❤️-red)

**Your Ultimate Study Companion 🚀**

*A premium, full-stack web application combining habit tracking, exam preparation, task management, and visual progress monitoring—all in one beautiful interface.*

[Live Demo](#-live-demo) • [Features](#-features) • [Installation](#-installation) • [Documentation](#-documentation) • [Contributing](#-contributing)

</div>

---

## 🌟 Overview

**Habit & Exam Tracker** is a comprehensive web application designed specifically for students who want to organize their academic life, build productive habits, prepare for exams effectively, and track their progress—all from a single dashboard.

Instead of juggling multiple apps for habit tracking, task management, exam planning, and note-taking, our platform brings everything together with a modern, responsive, and beautifully animated interface.

### Why Choose This Project?

✅ **All-in-One Solution** - Habits, exams, tasks, books, movies—everything in one place  
✅ **Premium UI/UX** - Parallax effects, smooth animations, dark/light mode  
✅ **Fully Responsive** - Works perfectly on desktop, tablet, and mobile  
✅ **Secure Authentication** - Login/signup with JWT tokens and password encryption  
✅ **Admin Dashboard** - Manage all users and data from a centralized panel  
✅ **Visual Tracking** - Kanban board, interactive calendar, progress bars  
✅ **CRUD Operations** - Add, edit, delete, and modify everything  
✅ **Cloud Ready** - Deploy on Vercel with MongoDB Atlas  
✅ **Open Source** - Free to use, modify, and extend  

---

## 🎯 Features

### 👤 User Authentication
- Secure login and signup system
- JWT token-based authentication
- Admin role with secret key access
- Password encryption with bcrypt
- Session management

### 📊 Habit Tracker
- Add unlimited habits (reading, exercise, coding, etc.)
- Daily check-ins and streak counting
- Progress visualization with statistics
- Mark habits as complete
- Edit and delete habits anytime

### 📚 Exam Preparation Guide
- Create exams with subject names and dates
- Track syllabus completion percentage
- Add topics and mark them as completed
- Automatic calculation of time remaining until exam
- Mark entire exam as complete
- Visual progress bars for each exam

### ✅ Daily Task Manager
- Add tasks with descriptions
- Mark tasks as complete/incomplete
- Organize tasks with priority levels
- Drag-and-drop reordering
- Edit and delete tasks
- Due date tracking

### 📖 Book Tracker
- Add books you want to read
- Track reading progress
- Mark books as completed
- Delete books from your list
- Fully editable tracker

### 🎬 Movie Tracker
- Add movies to your watch list
- Track watched movies
- Mark movies as completed
- Easy editing and deletion
- Maintain your entertainment list

### 📋 Visual Boards & Views
- **Kanban Board** - Organize tasks into "To Do", "In Progress", and "Completed" columns
- **Interactive Calendar** - View all exams and important dates at a glance
- **Task Cards** - Beautiful card-based interface for all items
- **Progress Analytics** - Visual statistics and progress tracking

### 🛡️ Admin Panel
- Manage all registered users
- View comprehensive user statistics
- Edit and delete user data globally
- Dashboard analytics
- User management interface
- View all habits, exams, tasks, books, and movies across all users

### 🎨 Premium UI/UX
- Modern parallax effects on landing page
- Smooth transitions and animations throughout
- Responsive design for all screen sizes
- Dark and light theme toggle
- Gradient backgrounds and premium colors
- Accessibility-friendly design
- Keyboard navigation support

### 🦶 Beautiful Footer
- Custom footer with "Made with love by Bhav"
- Present on all pages

---

## 🛠️ Tech Stack

### Frontend
- **React.js** - UI framework
- **Tailwind CSS** - Utility-first CSS
- **Bootstrap** - Responsive components
- **React Router** - Navigation
- **Axios** - HTTP client
- **React Icons** - Icon library
- **Framer Motion** - Animations
- **React Calendar** - Calendar integration

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** - ODM for MongoDB
- **JWT (jsonwebtoken)** - Authentication
- **bcryptjs** - Password hashing
- **dotenv** - Environment variables
- **CORS** - Cross-origin requests

### Deployment
- **Vercel** - Frontend and backend hosting
- **MongoDB Atlas** - Cloud database
- **GitHub** - Version control

---

## 📦 Installation

### Prerequisites
Before you begin, ensure you have the following installed:
- Node.js (v14 or higher)
- npm or yarn
- Git
- MongoDB (local or MongoDB Atlas account)

### Clone the Repository
```bash
git clone https://github.com/BhavAnsh/habit-exam-tracker.git
cd habit-exam-tracker
```

### Frontend Setup

```bash
# Navigate to frontend folder
cd frontend

# Install dependencies
npm install

# Create .env.local file
echo "VITE_API_URL=http://localhost:3001/api" > .env.local

# Start development server
npm run dev
```

The frontend will run on `http://localhost:5173`

### Backend Setup

```bash
# Navigate to backend folder (from root)
cd backend

# Install dependencies
npm install

# Create .env file
cat > .env << EOF
MONGODB_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/<dbname>?retryWrites=true&w=majority
JWT_SECRET=your_jwt_secret_key_here
ADMIN_SECRET_KEY=your_admin_secret_key_here
PORT=3001
NODE_ENV=development
EOF

# Start server
npm start
```

The backend will run on `http://localhost:3001`

### Environment Variables

#### Frontend (.env.local)
```env
VITE_API_URL=http://localhost:3001/api
```

#### Backend (.env)
```env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
ADMIN_SECRET_KEY=admin_secret_key_for_registration
PORT=3001
NODE_ENV=development
```

---

## 🚀 Quick Start

1. **Sign Up**: Create a new account (user or admin with secret key)
2. **Dashboard**: See your personalized dashboard after login
3. **Add Habits**: Click "Add Habit" and start tracking
4. **Create Exams**: Add exams with subjects, dates, and syllabus
5. **Daily Tasks**: Manage your daily to-do list
6. **Track Progress**: Use Kanban board and calendar to visualize your progress
7. **Admin Access**: Log in as admin to manage all users

---

## 📊 Project Structure

```
habit-exam-tracker/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   ├── HabitTracker.jsx
│   │   │   ├── ExamPlanner.jsx
│   │   │   ├── TaskManager.jsx
│   │   │   ├── KanbanBoard.jsx
│   │   │   ├── Calendar.jsx
│   │   │   ├── AdminPanel.jsx
│   │   │   └── Footer.jsx
│   │   ├── pages/
│   │   │   ├── LoginPage.jsx
│   │   │   ├── SignupPage.jsx
│   │   │   └── DashboardPage.jsx
│   │   ├── services/
│   │   │   └── api.js
│   │   ├── styles/
│   │   │   └── tailwind.css
│   │   └── App.jsx
│   ├── package.json
│   └── vite.config.js
│
├── backend/
│   ├── models/
│   │   ├── User.js
│   │   ├── Habit.js
│   │   ├── Exam.js
│   │   ├── Task.js
│   │   ├── Book.js
│   │   └── Movie.js
│   ├── routes/
│   │   ├── auth.js
│   │   ├── habits.js
│   │   ├── exams.js
│   │   ├── tasks.js
│   │   ├── books.js
│   │   ├── movies.js
│   │   └── admin.js
│   ├── middleware/
│   │   ├── auth.js
│   │   └── adminCheck.js
│   ├── controllers/
│   │   └── (controller files)
│   ├── server.js
│   ├── .env
│   └── package.json
│
└── README.md
```

---

## 📚 API Documentation

### Authentication Endpoints
```
POST   /api/auth/signup      - Register a new user
POST   /api/auth/login       - Login user
GET    /api/auth/me          - Get current user
POST   /api/auth/logout      - Logout user
```

### Habit Endpoints
```
GET    /api/habits           - Get all habits
POST   /api/habits           - Create new habit
PUT    /api/habits/:id       - Update habit
DELETE /api/habits/:id       - Delete habit
PUT    /api/habits/:id/mark  - Mark habit complete
```

### Exam Endpoints
```
GET    /api/exams            - Get all exams
POST   /api/exams            - Create new exam
PUT    /api/exams/:id        - Update exam
DELETE /api/exams/:id        - Delete exam
PUT    /api/exams/:id/mark   - Mark exam complete
```

### Task Endpoints
```
GET    /api/tasks            - Get all tasks
POST   /api/tasks            - Create new task
PUT    /api/tasks/:id        - Update task
DELETE /api/tasks/:id        - Delete task
PUT    /api/tasks/:id/mark   - Toggle task completion
```

### Book & Movie Endpoints
```
GET    /api/books            - Get all books
POST   /api/books            - Create new book
PUT    /api/books/:id        - Update book
DELETE /api/books/:id        - Delete book

GET    /api/movies           - Get all movies
POST   /api/movies           - Create new movie
PUT    /api/movies/:id       - Update movie
DELETE /api/movies/:id       - Delete movie
```

### Admin Endpoints
```
GET    /api/admin/users      - Get all users
GET    /api/admin/stats      - Get app statistics
PUT    /api/admin/users/:id  - Edit user
DELETE /api/admin/users/:id  - Delete user
```

---

## 🌐 Live Demo

Check out the live version here: [https://habit-exam-tracker.vercel.app](https://habit-exam-tracker.vercel.app)

**Demo Credentials:**
- **Email:** demo@example.com
- **Password:** demo123

---

## 📸 Screenshots

### Login Page
Beautiful authentication interface with admin toggle option.

### Dashboard
Personalized dashboard showing all your trackers at a glance.

### Habit Tracker
Track your daily habits with streaks and statistics.

### Exam Planner
Manage exams with syllabus tracking and time remaining calculation.

### Kanban Board
Organize tasks visually with drag-and-drop functionality.

### Calendar View
See all exams and important dates in calendar format.

### Admin Panel
Comprehensive admin dashboard to manage all users and data.

---

## 🚀 Deployment on Vercel

### Frontend Deployment

1. **Push to GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **Connect to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Select the `frontend` folder as root
   - Add environment variables (.env.local)
   - Click "Deploy"

3. **Update Backend URL**
   - In frontend `.env.local`, update `VITE_API_URL` to your Vercel backend URL

### Backend Deployment

1. **Create Separate Backend Repository** (or use the same repo with different folder)

2. **Deploy to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Create new project for backend
   - Set root directory to `backend/`
   - Add environment variables:
     - `MONGODB_URI` (MongoDB Atlas connection string)
     - `JWT_SECRET` (your secret key)
     - `ADMIN_SECRET_KEY` (admin registration key)
     - `PORT` (3001)
   - Deploy

3. **Update MongoDB**
   - Go to [MongoDB Atlas](https://www.mongodb.com/atlas)
   - Create free cluster
   - Get connection string
   - Add to backend `.env` file

---

## 🎓 Learning Resources

### For Beginners
- [React Documentation](https://react.dev)
- [Express.js Guide](https://expressjs.com)
- [MongoDB Tutorial](https://docs.mongodb.com/manual)
- [Tailwind CSS Docs](https://tailwindcss.com/docs)

### Advanced Topics
- [JWT Authentication](https://jwt.io)
- [RESTful API Design](https://restfulapi.net)
- [MERN Stack Tutorial](https://www.mongodb.com/mern-stack)
- [Vercel Deployment Guide](https://vercel.com/docs)

---

## 🤝 Contributing

We welcome contributions! Here's how to get started:

1. **Fork the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/habit-exam-tracker.git
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```

4. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
   ```

5. **Open a Pull Request**

### Contribution Ideas
- Add real-time notifications
- Implement social features (share progress with friends)
- Add AI-powered study recommendations
- Create mobile app version
- Add data export (PDF/Excel)
- Implement advanced analytics
- Add voice commands
- Create collaborative study groups feature

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 💬 Support & Feedback

Have questions or suggestions? We'd love to hear from you!

- **Issues**: [GitHub Issues](https://github.com/BhavAnsh/habit-exam-tracker/issues)
- **Discussions**: [GitHub Discussions](https://github.com/BhavAnsh/habit-exam-tracker/discussions)
- **Email**: support@habittrackerapp.com
- **Twitter**: [@HabitTrackerApp](https://twitter.com/HabitTrackerApp)

---

## 🙏 Acknowledgments

- Special thanks to the React, Node.js, and MongoDB communities
- Inspired by popular habit trackers and productivity apps
- Built with ❤️ for students everywhere
- Thanks to all contributors and supporters

---

## 📊 Stats

![Views](https://komarev.com/ghpvc/?username=BhavAnsh&label=Repository+Views&color=0e75b6&style=flat)

---

## 🌟 Show Your Support

If you find this project helpful, please give it a ⭐ on GitHub! Your support means a lot to us.

```
If this project helped you, consider:
- ⭐ Starring the repository
- 🍴 Forking for your own use
- 📢 Sharing with your friends
- 💬 Providing feedback and suggestions
```

---

<div align="center">

### Made with ❤️ by Bhav

**Happy Tracking! 🚀**

[⬆ Back to Top](#-allin-one-habit--exam-preparation-tracker)

</div>
