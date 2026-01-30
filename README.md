# 🎯 CUET Lost & Found Box

A comprehensive, smart web-based Lost and Found Management System designed for CUET (Chittagong University of Engineering & Technology) to help students and staff efficiently report, search, and recover lost items.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technology Stack](#technology-stack)
- [Getting Started](#getting-started)
- [User Guide](#user-guide)
- [Admin Guide](#admin-guide)
- [Pages Overview](#pages-overview)
- [Development](#development)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## 🌟 Overview

The CUET Lost & Found Box is a modern, colorful, and user-friendly web application that streamlines the process of reporting and finding lost items on campus. With an intuitive interface, powerful search capabilities, and role-based access control, it provides a complete solution for managing lost and found items.

### Key Highlights

- 🎨 **Beautiful UI**: Modern, colorful design with smooth animations
- 📱 **Fully Responsive**: Works seamlessly on desktop, tablet, and mobile devices
- 🔒 **Secure Authentication**: User registration, login, and role-based access
- 🔍 **Advanced Search**: Powerful filtering and search capabilities
- 👥 **Role-Based System**: User, Admin, and Super Admin roles
- ✅ **Item Approval Workflow**: Admin review process for all submissions
- 📊 **Dashboard Analytics**: Statistics and insights for admins
- 🌈 **Eye-Soothing Colors**: Carefully chosen color palette for comfort

## ✨ Features

### For Regular Users

- **User Registration & Login**
  - Secure account creation with email verification
  - Role selection (Student/Staff/Faculty)
  - Password-protected accounts

- **Report Lost Items**
  - Detailed form with item information
  - Optional image upload with preview
  - Location and date tracking
  - Contact information management

- **Report Found Items**
  - Similar form structure to lost items
  - Required image upload
  - Storage location specification
  - Immediate admin notification

- **Search & Browse**
  - Live feed of approved items
  - Advanced filtering (category, date, location, status)
  - Grid/List view toggle
  - Item detail modal with full information
  - Contact request functionality

- **User Dashboard**
  - View all submitted items
  - Track item status (pending/approved/rejected)
  - Edit or delete own submissions
  - Personal statistics

### For Admins

- **Admin Panel**
  - Dashboard with system statistics
  - Pending, approved, and rejected items tabs
  - Review and approve/reject submissions
  - Rejection reason tracking
  - Item detail view with full history

- **Item Management**
  - Approve or reject submissions
  - Edit item details
  - Delete items
  - Search and filter across all items

### For Super Admins

- **User Management**
  - View all registered users
  - Promote users to admin
  - Demote admins to users
  - Monitor user activity
  - User statistics

- **System Overview**
  - Complete system statistics
  - User role distribution
  - Item approval rates
  - Activity monitoring

## 📁 Project Structure

```
CUET LOST & FOUND BOX/
│
├── Frontend/                    # Frontend application
│   ├── index.html              # Landing/Home page
│   ├── login.html              # User login page
│   ├── register.html           # User registration page
│   ├── feed.html               # Live feed of items
│   ├── search.html             # Advanced search page
│   ├── report-lost.html        # Report lost item form
│   ├── report-found.html       # Report found item form
│   ├── user-dashboard.html     # User personal dashboard
│   ├── admin.html              # Admin panel
│   ├── super-admin.html        # Super admin panel
│   ├── QUICKSTART.html         # Quick start guide
│   │
│   ├── css/                    # Stylesheets
│   │   ├── style.css           # Main styles
│   │   └── auth.css            # Authentication page styles
│   │
│   ├── js/                     # JavaScript files
│   │   ├── main.js             # Common utilities & navigation
│   │   ├── auth.js             # Authentication logic
│   │   ├── feed.js             # Feed page functionality
│   │   ├── search.js           # Search & filter logic
│   │   ├── report.js           # Form validation & submission
│   │   ├── user-dashboard.js   # User dashboard logic
│   │   ├── admin.js            # Admin panel functionality
│   │   └── super-admin.js      # Super admin panel logic
│   │
│   ├── resources/              # Images and assets
│   │
│   └── README.md               # Frontend documentation
│
├── Backend/                     # Backend (To be implemented)
│
└── README.md                    # This file
```

## 🛠 Technology Stack

### Frontend

- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with CSS Grid and Flexbox
  - CSS Variables for theming
  - Smooth animations and transitions
  - Responsive design with media queries
- **Vanilla JavaScript (ES6+)**: 
  - DOM manipulation
  - LocalStorage for data persistence (demo)
  - Form validation
  - Dynamic content rendering
  - Event handling

### Planned Backend

- **Framework Options**: Django, FastAPI, Node.js/Express
- **Database**: PostgreSQL or MongoDB
- **Authentication**: JWT tokens
- **Image Storage**: AWS S3 or Cloudinary
- **Email Service**: SendGrid or AWS SES

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- A local web server (optional but recommended)
- Text editor or IDE (VS Code recommended)

### Installation

1. **Download or Clone the Project**
   ```bash
   git clone <repository-url>
   cd "CUET LOST & FOUND BOX"
   ```

2. **Open with a Web Server**

   **Option 1: Using Python**
   ```bash
   cd Frontend
   # Python 3
   python -m http.server 8000
   # Then open http://localhost:8000 in your browser
   ```

   **Option 2: Using Node.js**
   ```bash
   cd Frontend
   npx http-server -p 8000
   # Then open http://localhost:8000 in your browser
   ```

   **Option 3: Using VS Code Live Server**
   - Install the "Live Server" extension
   - Right-click on `index.html`
   - Select "Open with Live Server"

3. **Or Open Directly**
   - Navigate to `Frontend` folder
   - Double-click `index.html`
   - Note: Some features work better with a local server

### Quick Start

Visit [QUICKSTART.html](Frontend/QUICKSTART.html) for an interactive quick start guide.

## 📖 User Guide

### Registration

1. Navigate to [register.html](Frontend/register.html)
2. Fill in your details:
   - Full Name
   - Email (CUET email recommended)
   - Phone Number
   - Student/Staff ID
   - Role (Student/Staff/Faculty)
   - Password (min 8 characters)
3. Click "Create Account"
4. Login with your credentials

### Login

1. Visit [login.html](Frontend/login.html)
2. Enter your email and password
3. Click "Login"
4. You'll be redirected based on your role

### Reporting a Lost Item

1. Click "Report Lost" in navigation
2. Fill in the form:
   - Item Name *
   - Category (Electronics, Documents, etc.)
   - Description *
   - Last Seen Location *
   - Date and Time *
   - Your Contact Information
   - Upload Image (optional)
3. Click "Submit Report"
4. Wait for admin approval

### Reporting a Found Item

1. Click "Report Found" in navigation
2. Fill in item details:
   - Item Name *
   - Category *
   - Description *
   - Found Location *
   - Date and Time Found *
   - Current Storage Location *
   - Upload Image (required)
   - Your Contact Information
3. Submit for review

### Searching for Items

1. Navigate to "Search Items" or "Feed"
2. Use the search bar for keywords
3. Apply filters:
   - Status: All/Lost/Found
   - Category: Select from dropdown
   - Date Range: From - To
   - Location: Specific campus location
4. Browse results in grid or list view
5. Click on items for detailed view
6. Request contact information if you find a match

### Managing Your Items

1. Go to "My Dashboard"
2. View your profile and statistics
3. See all your submissions organized by status:
   - Pending (awaiting approval)
   - Approved (visible to others)
   - Rejected (with reasons)
4. Edit or delete your items
5. Track item status changes

## 👨‍💼 Admin Guide

### Accessing Admin Panel

1. Login with an admin account
2. Navigate to "Admin Panel"
3. View dashboard statistics

### Reviewing Items

1. Click on "Pending Reviews" tab
2. View item details by clicking on cards
3. Review information, images, and contact details
4. Approve or Reject:
   - **Approve**: Item becomes visible to all users
   - **Reject**: Provide a reason for rejection

### Managing Approved Items

1. Click "Approved" tab
2. Search and filter items
3. Edit details if needed
4. Delete inappropriate items
5. Monitor item status

### Viewing Rejected Items

1. Click "Rejected" tab
2. Review rejection history
3. Re-approve if decision changes
4. View rejection reasons

## 🌐 Pages Overview

### Public Pages (No Login Required)

- **[index.html](Frontend/index.html)**: Landing page with hero section and features
- **[login.html](Frontend/login.html)**: User authentication
- **[register.html](Frontend/register.html)**: New user registration
- **[QUICKSTART.html](Frontend/QUICKSTART.html)**: Interactive guide

### User Pages (Login Required)

- **[feed.html](Frontend/feed.html)**: Live feed of all approved items
- **[search.html](Frontend/search.html)**: Advanced search with filters
- **[report-lost.html](Frontend/report-lost.html)**: Report lost item form
- **[report-found.html](Frontend/report-found.html)**: Report found item form
- **[user-dashboard.html](Frontend/user-dashboard.html)**: Personal dashboard

### Admin Pages (Admin Role Required)

- **[admin.html](Frontend/admin.html)**: Admin panel for item management

### Super Admin Pages (Super Admin Role Required)

- **[super-admin.html](Frontend/super-admin.html)**: User and system management

## 🎨 Design Features

### Color Scheme

The application uses a vibrant, eye-soothing color palette:

- **Primary**: #6366f1 (Indigo) - Main actions and highlights
- **Secondary**: #10b981 (Emerald) - Success and positive actions
- **Accent**: #f59e0b (Amber) - Warnings and attention
- **Danger**: #ef4444 (Red) - Errors and destructive actions
- **Info**: #3b82f6 (Blue) - Information and links

### UI Elements

- **Cards**: Rounded corners with subtle shadows
- **Buttons**: Gradient backgrounds with hover effects
- **Forms**: Clean, spacious layouts with validation
- **Modals**: Smooth fade-in animations
- **Animations**: Fade, slide, and scale transitions
- **Icons**: Emoji-based for universal recognition

### Responsive Design

- **Mobile First**: Optimized for mobile devices
- **Breakpoints**:
  - Mobile: < 768px
  - Tablet: 768px - 1023px
  - Desktop: ≥ 1024px
- **Adaptive Navigation**: Hamburger menu on mobile
- **Flexible Grids**: Adjusts from 1 to 4 columns

## 💻 Development

### File Organization

- **HTML**: Semantic, accessible markup
- **CSS**: Modular, reusable styles with CSS variables
- **JavaScript**: Organized by functionality, ES6+ syntax

### Key JavaScript Modules

#### main.js
- Navigation handling
- Authentication state management
- Common utilities
- Mock data (for demo)

#### auth.js
- Login/Registration logic
- Form validation
- Password strength checking
- User session management

#### feed.js & search.js
- Item filtering and search
- Dynamic rendering
- Modal handling
- View toggling

#### report.js
- Form validation
- Image upload and preview
- Data submission
- Success/error handling

#### user-dashboard.js
- Personal item management
- Statistics display
- Edit/delete functionality

#### admin.js
- Item approval workflow
- Admin dashboard
- Bulk operations
- Status filtering

#### super-admin.js
- User management
- Role assignment
- System statistics
- User activity monitoring

### LocalStorage Structure

Current implementation uses browser LocalStorage for demo purposes:

```javascript
// Users
localStorage.setItem('users', JSON.stringify([
    {
        id: 1,
        name: "John Doe",
        email: "john@cuet.ac.bd",
        phone: "01712345678",
        studentId: "1234567",
        role: "user", // user, admin, superadmin
        password: "hashed_password"
    }
]));

// Items
localStorage.setItem('items', JSON.stringify([
    {
        id: 1,
        type: "lost", // lost or found
        name: "iPhone 13",
        category: "Electronics",
        description: "Black iPhone with broken screen",
        location: "Library - 2nd Floor",
        date: "2026-01-25",
        time: "14:30",
        contactName: "John Doe",
        email: "john@cuet.ac.bd",
        phone: "01712345678",
        image: "base64_or_url",
        status: "pending", // pending, approved, rejected
        submittedBy: 1,
        submittedAt: "2026-01-25T14:35:00Z",
        rejectionReason: ""
    }
]));
```

## 🔮 Future Enhancements

### Backend Integration

- [ ] RESTful API development
- [ ] Database schema implementation
- [ ] User authentication with JWT
- [ ] File upload to cloud storage
- [ ] Email notifications
- [ ] SMS notifications (optional)

### Additional Features

- [ ] Real-time notifications (WebSocket)
- [ ] Email verification on registration
- [ ] Password reset functionality
- [ ] Two-factor authentication
- [ ] Item claim workflow
- [ ] Match suggestions (AI-powered)
- [ ] QR code generation for items
- [ ] Export reports (PDF/Excel)
- [ ] Analytics dashboard
- [ ] Mobile app (React Native/Flutter)

### Enhancements

- [ ] Multi-language support
- [ ] Dark mode
- [ ] Accessibility improvements (WCAG compliance)
- [ ] Progressive Web App (PWA)
- [ ] Image compression and optimization
- [ ] Advanced search with autocomplete
- [ ] Social media sharing
- [ ] Item expiry and auto-archival
- [ ] Rating and feedback system

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Coding Standards

- Use meaningful variable and function names
- Comment complex logic
- Follow existing code style
- Test on multiple browsers
- Ensure responsive design
- Validate HTML/CSS
- Use ES6+ JavaScript features

## 📄 License

This project is created for educational purposes as part of the CUET Lost & Found Box initiative.

## 👥 Authors

Developed for Chittagong University of Engineering & Technology (CUET)

## 🙏 Acknowledgments

- Modern web design principles
- Responsive design best practices
- Vanilla JavaScript patterns
- CSS Grid and Flexbox layouts
- Community feedback and testing

## 📞 Support

For support, please contact:
- Email: support@cuet-lostfound.edu.bd
- Campus Help Desk: IT Office, CUET

## 🔗 Related Documentation

- [Frontend README](Frontend/README.md) - Detailed frontend documentation
- [Quick Start Guide](Frontend/QUICKSTART.html) - Interactive guide for new users

---

**Current Status**: Frontend Complete | Backend In Progress

**Version**: 1.0.0

**Last Updated**: January 31, 2026

---

Made with ❤️ for CUET Community
