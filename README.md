---

# Study Notion

**Study Notion** is a comprehensive EdTech platform built using the **MERN stack**. It is designed to cater to two distinct user roles, **Instructors** and **Students**, each with their own customized user interface and functionalities. The platform also incorporates **OTP-based verification** for secure user registration. The application is deployed with the **frontend on Vercel** and the **backend on Render**.

## Features

### 1. **User Roles**
   - **Instructors:**
     - Can create courses.
     - Track the progress of students who have purchased their courses.
     - Instructors are restricted to create courses only under categories specified by the Admin.
   - **Students:**
     - Can view all available courses.
     - Purchase courses and track their progress.
     - Can access purchased course content.

### 2. **Role of Admin**
   - **Admin** creates course categories.
   - Instructors are limited to creating courses under these predefined categories.
   - Ensures proper organization and maintenance of the course catalog.

### 3. **OTP-Based Verification**
   - Secure user registration by verifying email with a One-Time Password (OTP).
   - Only verified users can register on the platform.

### 4. **Course Management**
   - **Course Creation:** Instructors create and upload course content (videos, resources).
   - **Progress Tracking:** Students and Instructors can track course progress.

### 5. **Tech Stack**
   - **Frontend:** React.js, Redux, CSS, and Axios for API requests.
   - **Backend:** Node.js, Express.js, MongoDB.
   - **Database:** MongoDB stores user information, course details, and student progress.
   - **Media Management:** Cloudinary is integrated to handle media uploads such as course videos and images.

## Project Structure

The project is divided into two main parts: **Frontend** and **Backend**. Below is an explanation of the folder structure for both.

### Frontend

Located in the `src/` folder.

- **Components:** Contains reusable components like buttons, forms, and layout elements.
- **Pages:** Includes pages like the course list, course creation, user dashboard, and login/signup.
- **Services:** Manages API calls related to authentication, course creation, and student progress.
- **Redux Slices:** Handles application state using Redux for authentication, courses, and user roles.
- **Hooks:** Custom hooks to abstract logic, such as handling forms or fetching data.
- **Assets:** Stores static assets like images, fonts, etc.

### Backend

Located in the `server/` folder.

- **Config:** Holds configuration files like database setup, environment variables, etc.
- **Controllers:** Handles the core business logic such as course creation, student registration, and progress tracking.
- **Routes:** Defines the API endpoints, e.g., `/api/users`, `/api/courses`.
- **Models:** Schema definitions for MongoDB collections (User, Course, Category).
- **Middleware:** Custom middlewares like authentication checks, error handling, etc.
- **Utils:** Contains helper functions such as email verification utilities for OTP.

## Deployment

The project is deployed using **Vercel** for the frontend and **Render** for the backend.

- **Frontend:** [Study Notion Frontend](https://study-notion-frontend-1nresh692-neha-singhals-projects.vercel.app/)
- **Backend:** [Study Notion Backend](https://study-notion-backend-l79z.onrender.com)

## Getting Started

To run the project locally, follow these steps:

### Prerequisites

- Node.js installed on your local machine.
- MongoDB setup locally or using a cloud service like MongoDB Atlas.
- Cloudinary account for managing media uploads.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Neha-Singhal-0/Study-Notion.git
   ```

2. Install dependencies:

   For the backend:

   ```bash
   cd server
   npm install
   ```

   For the frontend:

   ```bash
   npm install
   ```

3. Set up environment variables:

   Create a `.env` file in the `server` directory and add the following variables:

   ```bash
   PORT=5000
   MONGO_URI=<your_mongo_db_uri>
   JWT_SECRET=<your_jwt_secret>
   CLOUDINARY_CLOUD_NAME=<your_cloudinary_name>
   CLOUDINARY_API_KEY=<your_cloudinary_api_key>
   CLOUDINARY_API_SECRET=<your_cloudinary_api_secret>
   ```

4. Run the development server:

   For backend:

   ```bash
   npm run dev
   ```

   For frontend:

   ```bash
   npm start
   ```

5. Visit `http://localhost:3000` to view the application.

## Technologies Used

- **React.js**: For building the user interface and creating reusable UI components.
- **Redux**: For state management across the entire app.
- **Node.js**: Handles backend services, including user authentication and course management.
- **Express.js**: Web framework for creating API routes and handling server logic.
- **MongoDB**: NoSQL database for storing user, course, and category data.
- **Cloudinary**: Media management tool for handling course video and image uploads.
- **Axios**: For making HTTP requests to the backend from the frontend.
- **JWT**: JSON Web Tokens for handling user authentication and authorization.

## Conclusion

**Study Notion** provides an integrated platform for online learning with instructor-student interaction. It ensures a seamless experience for both instructors creating courses and students consuming the content, all while maintaining secure user verification and progress tracking.

Feel free to explore the platform and contribute!

--- 
