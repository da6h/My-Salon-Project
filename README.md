# 💼 My-Salon-Project

Full-stack web application for salon booking and service management with Node.js backend and responsive HTML/CSS/JavaScript frontend.

## ✨ Key Features

### 👥 Customer Portal
- 🔍 Browse available salon services
- 📅 Create and manage bookings
- ✏️ Edit existing appointments
- ❌ Cancel bookings
- 📱 Automatic phone number confirmation
- 🎨 Clean, responsive user interface

### 🛠️ Admin Dashboard
- 📊 View all customer bookings
- 👤 Track bookings per employee
- ✏️ Edit and update appointments
- 🗑️ Cancel or delete bookings
- 📈 Centralized booking management
- 🔄 Real-time data synchronization

### ⚙️ Backend System
- 🚀 RESTful API architecture
- ✅ Full CRUD operations for bookings
- 🔒 Centralized validation and error handling
- 📁 Clean, modular code structure
- 🔀 Separate routes for admin and customer actions

## 🛠️ Tech Stack

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **RESTful API** - Architecture pattern

### Frontend
- **HTML5** - Structure
- **CSS3** - Styling and responsive design
- **JavaScript** - Client-side functionality

### Tools
- **Git** - Version control
- **npm** - Package management

## 📁 Project Structure
```
salon-system/
│
├── Server/                    # Backend
│   ├── src/
│   │   ├── routes/           # API routes (client + admin)
│   │   ├── lib/              # Helpers, database utilities
│   │   └── app.js            # Main server file
│   └── package.json
│
├── frontend/                  # Frontend
│   ├── index.html            # Main booking page
│   ├── confirm.html          # Confirmation page
│   ├── admin/                # Admin dashboard
│   └── assets/               # CSS, JS, images
│
├── .gitignore
└── README.md
```

## 🚀 Installation & Setup

### Prerequisites
- Node.js (v14 or higher)
- npm (Node Package Manager)

### Installation Steps

**1. Clone the repository**
```bash
git clone https://github.com/da6h/My-Salon-Project.git
cd My-Salon-Project
```

**2. Install backend dependencies**
```bash
cd Server
npm install
```

**3. Start the development server**
```bash
npm start
```

**4. Access the application**
```
Frontend: http://localhost:5000
Admin Panel: http://localhost:5000/admin
```

## 🔌 API Documentation

### Customer Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/bookings` | Create a new booking |
| `GET` | `/bookings` | Retrieve all customer bookings |
| `PUT` | `/bookings/:id` | Update existing booking |
| `DELETE` | `/bookings/:id` | Cancel/delete booking |

### Admin Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/admin/bookings` | View all bookings |
| `GET` | `/admin/employees/:id/bookings` | View employee-specific bookings |
| `PUT` | `/admin/bookings/:id` | Edit/update any booking |
| `DELETE` | `/admin/bookings/:id` | Cancel/delete any booking |

## 💡 How It Works

### Customer Booking Flow
1. Customer browses available services
2. Selects desired service and time slot
3. Enters contact information
4. Receives booking confirmation with details
5. Can edit or cancel booking as needed

### Admin Management
1. Admin logs into dashboard
2. Views all bookings in centralized panel
3. Can filter by employee or date
4. Manages bookings (edit/cancel)
5. System updates reflect in real-time

## 📚 What I Learned

Building this project taught me:
- **Backend Development**: Creating RESTful APIs with Node.js and Express
- **Server Architecture**: Organizing routes, middleware, and business logic
- **CRUD Operations**: Implementing Create, Read, Update, Delete functionality
- **Error Handling**: Centralized validation and error management
- **Frontend Integration**: Connecting client-side JavaScript with backend APIs
- **Async Programming**: Working with promises and async/await patterns
- **API Design**: Separating customer and admin endpoints
- **Code Organization**: Maintaining clean, modular project structure


## 🐛 Known Issues & Limitations

- Currently uses in-memory data storage (resets on server restart)
- No persistent database implementation yet
- Limited user authentication
- Basic error handling on frontend

## 🧪 Testing

To test the application:

1. **Customer Flow**:
   - Navigate to `http://localhost:5000`
   - Create a test booking
   - Verify confirmation page

2. **Admin Flow**:
   - Navigate to `http://localhost:5000/admin`
   - View created bookings
   - Test edit/delete functionality

---

## ⭐ Acknowledgments

Built as part of Software Engineering studies to demonstrate:
- Full-stack web development skills
- RESTful API design
- Frontend-backend integration
- Clean code practices

---

**⭐ If you find this project helpful, please consider giving it a star!**


