# MIT Info Site

A comprehensive React-based institutional information and management system designed for educational institutions. This project provides a public-facing website combined with role-based dashboards for students, staff, and administrators.

## Project Overview

The MIT Info Site serves as both a digital presence for the institution and an integrated management system for academic and administrative operations. It features a modern, responsive design with smooth animations and intuitive navigation.

### Key Features

#### Public Pages
- **Landing Page**: Eye-catching hero section with institution overview
- **About Section**: Detailed information about the institution
- **Departments**: Browse academic departments and their details
- **Labs**: Information about research and laboratory facilities
- **News & Updates**: Latest news and announcements
- **Alumni Network**: Alumni information and connections
- **Gallery**: Visual showcase of campus and events
- **Admissions**: Application information and process
- **Contact**: Contact information and inquiry form

#### Role-Based Dashboards
- **Student Dashboard**: View grades, projects, attendance records, and personalized notices
- **Staff Dashboard**: Manage student attendance, post notices, view event calendars
- **Admin Dashboard**: Full system management including user roles, departments, events, and notices

#### Core Features
- **Authentication**: Multi-role login system (Student, Staff, Admin)
- **Attendance Tracking**: Track and manage student attendance
- **Notice System**: Publish and manage notices across roles
- **Project Management**: View and manage student projects
- **Event Calendar**: Schedule and manage institutional events
- **Role-Based Access Control**: Secure access to role-specific features

## Tech Stack

- **Frontend Framework**: React 18.2.0
- **Routing**: React Router DOM 6.30.1
- **Styling**: Tailwind CSS + PostCSS
- **Animations**: Framer Motion 12.18.1
- **Icons**: React Icons 5.5.0, Lucide React 0.515.0
- **Gallery**: Yet Another React Lightbox 3.23.2
- **Testing**: React Testing Library, Jest
- **Build Tool**: Create React App with React Scripts

## Project Structure

```
src/
├── components/           # Reusable UI components
│   ├── About.jsx
│   ├── Alumni.jsx
│   ├── Contact.jsx
│   ├── Departments.jsx
│   ├── Labs.jsx
│   ├── Landing.jsx
│   ├── Navbar.jsx
│   ├── News.jsx
│   ├── Admin/            # Admin dashboard components
│   ├── Staff/            # Staff dashboard components
│   ├── Students/         # Student dashboard components
│   └── Shared/           # Shared components
├── pages/                # Page components
│   ├── Admissions.jsx
│   ├── DepartmentsPage.jsx
│   ├── Gallery.jsx
│   ├── Home.jsx
│   ├── Login.jsx
│   └── Projects.jsx
├── context/              # React Context for state management
│   └── AttendanceContext.js
├── data/                 # Static data
│   └── students.js
├── App.js                # Main app routing
└── index.js              # Entry point
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone <repository-url>
cd mit-info-site-master
```

2. Install dependencies
```bash
npm install
```

### Available Scripts

#### Development
```bash
npm start
```
Runs the app in development mode. Open [http://localhost:3000](http://localhost:3000) to view it in your browser.
The page reloads when you make changes, and lint errors appear in the console.

#### Testing
```bash
npm test
```
Launches the test runner in interactive watch mode.

#### Build for Production
```bash
npm run build
```
Builds the app for production to the `build` folder. The build is minified and optimized for best performance.

## Authentication

The application includes built-in authentication with the following demo credentials:

| Role | Username | Password |
|------|----------|----------|
| Student | student001 | student123 |
| Staff | staff001 | staff123 |
| Admin | admin001 | admin123 |

> **Note**: This is a demo implementation. For production, integrate with a proper authentication system (JWT, OAuth, etc.)

## Routes

### Public Routes
- `/` - Home page with all public sections
- `/gallery` - Photo gallery
- `/admissions` - Admissions information
- `/departments` - Departments listing
- `/projects` - Projects showcase

### Authentication
- `/login` - Login page for all roles

### Protected Routes
- `/dashboard/student` - Student dashboard
- `/dashboard/staff` - Staff dashboard
- `/dashboard/admin` - Admin dashboard
- `/dashboard/staff/students-attendance` - Attendance management

## Development Notes

- **State Management**: Uses React Context API via `AttendanceContext` for sharing attendance data across components
- **Animations**: Framer Motion is configured for smooth page transitions and component animations
- **Styling**: Tailwind CSS provides utility-first styling with responsive design
- **Icons**: Multiple icon libraries (React Icons + Lucide) for comprehensive icon coverage

## Future Enhancements

- Backend API integration for data persistence
- Production-ready authentication system
- Database integration
- Real-time notifications
- Email integration for notices and announcements
- Export/Import functionality for data
- Advanced analytics dashboard
- Mobile app version

## Contributing

Contributions are welcome. Please follow standard Git workflow and ensure code adheres to React and Tailwind CSS best practices.

## License

This project is part of the MIT institution's digital infrastructure.

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
