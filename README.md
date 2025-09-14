# Student Management System
This is my Student Management System project built with React + Node.js.


A responsive, professional web application for managing student information with a clean UI and comprehensive functionality.

## 🚀 Features

- **Dashboard**: Overview with student statistics and welcome message
- **Student List**: Searchable table displaying all student information
- **Add Student**: Form to create new student records
- **Delete Student**: Remove students with confirmation dialog
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Real-time Search**: Filter students by name, ID, email, or course
- **Professional UI**: Clean, modern interface built with Tailwind CSS

## 📋 Prerequisites

Before running this application, make sure you have the following installed:

- **Node.js** (version 14.0 or higher)
- **npm** (comes with Node.js) or **yarn**
- A modern web browser (Chrome, Firefox, Safari, Edge)

## 🛠️ Setup Instructions

### Option 1: Using Create React App (Recommended)

1. **Create a new React project**:
   ```bash
   npx create-react-app student-management-system
   cd student-management-system
   ```

2. **Install Tailwind CSS**:
   ```bash
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init -p
   ```

3. **Configure Tailwind CSS**:
   
   Replace the content of `tailwind.config.js`:
   ```javascript
   /** @type {import('tailwindcss').Config} */
   module.exports = {
     content: [
       "./src/**/*.{js,jsx,ts,tsx}",
     ],
     theme: {
       extend: {},
     },
     plugins: [],
   }
   ```

4. **Update CSS file**:
   
   Replace the content of `src/index.css`:
   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```

5. **Install Lucide React for icons**:
   ```bash
   npm install lucide-react
   ```

6. **Replace App.js**:
   
   Copy the StudentManagementSystem component code into `src/App.js`

### Option 2: Using Existing Project

1. **Clone or download** the project files
2. **Install dependencies**:
   ```bash
   npm install
   ```
   or
   ```bash
   yarn install
   ```

## 🏃‍♂️ Running the Application

### Development Mode

```bash
npm start
```
or
```bash
yarn start
```

The application will open in your browser at `http://localhost:3000`

### Production Build

```bash
npm run build
```
or
```bash
yarn build
```

This creates a `build` folder with optimized production files.

## 📱 Usage Guide

### Dashboard
- View total student count and statistics
- See breakdown of students by status (Active, Graduated, On Hold, Inactive)
- Get an overview of the system

### Students Page
- Browse all students in a searchable table
- Use the search bar to filter by name, student ID, email, or course
- View student details including contact information and enrollment status
- Delete students using the trash icon (requires confirmation)

### Add Student Page
- Fill in the form with required information:
  - First Name* (required)
  - Last Name* (required) 
  - Email* (required)
  - Phone (optional)
  - Course* (required - select from dropdown)
  - Status (defaults to Active)
- Click "Add Student" to create the record
- Use "Reset" to clear the form

## 🗂️ Project Structure

```
student-management-system/
├── public/
│   ├── index.html
│   └── ...
├── src/
│   ├── App.js                    # Main component
│   ├── index.js                  # Entry point
│   ├── index.css                 # Tailwind CSS imports
│   └── ...
├── package.json
├── tailwind.config.js
└── README.md
```

## 🔧 Technical Details

- **Frontend**: React 18+ with Hooks
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **Data Source**: DummyJSON API (https://dummyjson.com/users)
- **State Management**: React useState/useEffect
- **Responsive**: Mobile-first design approach

<<<<<<< HEAD
This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
>>>>>>> 1de65ae (Initialize project using Create React App)
=======
## 🌐 API Integration

The application fetches student data from `https://dummyjson.com/users` and transforms it to include:
- Student ID (auto-generated)
- Course assignment (randomly assigned from predefined list)
- Status (randomly assigned)
- Enrollment date (generated)

## 🔍 Testing

### Manual Testing Checklist

- [ ] Application loads without errors
- [ ] Dashboard displays correct statistics
- [ ] Student list loads and displays data
- [ ] Search functionality works across all fields
- [ ] Add student form validation works
- [ ] New students appear in the list after creation
- [ ] Delete confirmation modal appears
- [ ] Students are removed after confirmation
- [ ] Application is responsive on different screen sizes

### Browser Testing

Test the application in:
- [ ] Chrome
- [ ] Firefox
- [ ] Safari
- [ ] Edge

## 🚨 Troubleshooting

### Common Issues

1. **Application won't start**:
   - Ensure Node.js is installed (`node --version`)
   - Delete `node_modules` and run `npm install` again
   - Check for port conflicts (default: 3000)

2. **Styling issues**:
   - Verify Tailwind CSS is properly configured
   - Check `tailwind.config.js` content paths
   - Ensure CSS imports are correct in `index.css`

3. **API data not loading**:
   - Check internet connection
   - Verify console for CORS errors
   - API endpoint: https://dummyjson.com/users should be accessible

### Browser Console

Check browser developer console (F12) for any error messages if issues occur.

## 📄 License

This project is for educational/demonstration purposes.

## 🤝 Contributing

This is a demonstration project. For improvements, please create issues or submit pull requests.

---

**Note**: This application uses mock data from DummyJSON for demonstration purposes. In a production environment, you would connect to a real backend API with proper authentication and data persistence.
>>>>>>> cc79f7b (Initial commit - Student Management System)
