# Study Notion

**Study Notion** is a comprehensive EdTech platform that caters to both **Instructors** and **Students**. It provides distinct functionalities for each type of user, such as course creation and tracking for instructors, and course browsing and purchasing for students. The platform also features a secure OTP-based registration and a category-based course management system controlled by admins.

## Table of Contents
1. [Features](#features)
2. [Technologies Used](#technologies-used)
3. [Project Structure](#project-structure)
4. [Getting Started](#getting-started)
5. [Usage](#usage)
6. [Deployed Links](#deployed-links)
7. [Contributing](#contributing)
8. [License](#license)

## Features

### For Instructors:
- **Login and Signup with OTP Verification**: Users must verify their identity with an OTP to complete the signup process.
- **Course Creation**: Instructors can create courses, but they are restricted to creating courses in the categories defined by the admin.
- **Student Progress Tracking**: Instructors can track the progress of students who have purchased their courses.

### For Students:
- **View All Courses**: Students can browse all available courses.
- **Purchase Courses**: Students can purchase courses and access the course content.
- **Track Progress**: Students can see their progress through each course.

### For Admin:
- **Category Management**: Admins can create categories, and instructors are restricted to creating courses only within these admin-defined categories.

## Technologies Used

The project is built using the **MERN stack** with the following key technologies:

- **MongoDB**: NoSQL database used for storing user data, course information, and more.
- **Express.js**: Backend framework for building the REST API.
- **React.js**: Frontend library used to build a dynamic and interactive UI.
- **Node.js**: Backend runtime environment for running JavaScript on the server side.
- **Cloudinary**: Used for managing and storing media such as course images and videos.
- **JWT (JSON Web Tokens)**: Used for user authentication and authorization.
- **OTP-based Verification**: Secure signup process by sending an OTP to verify user identity.
- **Mongoose**: Object Data Modeling (ODM) library for MongoDB.
- **Tailwind CSS**: Utility-first CSS framework used to design a responsive and modern UI.
  
## Project Structure

The project follows an **MVC (Model-View-Controller)** architecture for maintainability and scalability. Below is an overview of the main directories:

### `/server`
- **config**: Database and other configurations.
- **controllers**: Contains the logic for handling requests.
- **mail/templates**: HTML email templates for OTP verification.
- **middlewares**: Custom middleware functions for authentication, authorization, etc.
- **models**: Mongoose models for MongoDB collections.
- **routes**: Express routes for API endpoints.
- **utils**: Utility functions like OTP generation and more.

### `/src`
- **assets**: Static files like images.
- **components**: React components for building the UI.
- **hooks**: Custom hooks to manage state and side effects.
- **pages**: React pages corresponding to different routes (e.g., login, signup, courses).
- **slices**: Redux slices for state management.
- **services**: API service files for communication between frontend and backend.

## Getting Started

To get the project up and running locally, follow these steps:

### Prerequisites

- Node.js installed on your machine
- MongoDB (you can use MongoDB Atlas or a local instance)
- Cloudinary account for media management

### Installation

1. **Clone the repository:**
   git clone https://github.com/Neha-Singhal-0/Study-Notion.git

# 2. Navigate to the project directory:
cd Study-Notion

# 3. Install dependencies for both frontend and backend:
# Install frontend dependencies
cd src
npm install

# Install backend dependencies
cd ../server
npm install

# 4. Set up environment variables:
# Create a .env file in the root of the /server directory and add the following:
MONGO_URI=<your-mongodb-uri>
JWT_SECRET=<your-jwt-secret>
CLOUDINARY_CLOUD_NAME=<your-cloudinary-cloud-name>
CLOUDINARY_API_KEY=<your-cloudinary-api-key>
CLOUDINARY_API_SECRET=<your-cloudinary-api-secret>

# 5. Start the development servers:
# Frontend (inside /src):
npm start

# Backend (inside /server):
npm run dev

# 6. Open your browser and navigate to:
# Frontend: http://localhost:3000
# Backend: http://localhost:5000


Usage
Instructor: Can log in, create courses, and track student progress.
Student: Can browse and purchase courses, and track their progress.
Admin: Can manage categories to restrict what courses instructors can create.


Deployed Links
Frontend: Study Notion Frontend on Vercel
Backend: Study Notion Backend on Render

Contributing
Contributions are welcome! If you’d like to contribute, please fork the repository and use a feature branch. Pull requests are warmly welcome.

Fork the repository
Create your feature branch: git checkout -b feature/your-feature-name
Commit your changes: git commit -m 'Add some feature'
Push to the branch: git push origin feature/your-feature-name
Open a pull request

License
This project is licensed under the MIT License - see the LICENSE file for details.
   
