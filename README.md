# SnapSkillzz Learning Platform Server

This repository contains the server-side code for SnapSkillzz, an online learning platform designed to facilitate course management and user engagement. The platform distinguishes between administrators and users, providing distinct functionalities for each.

## Project Overview

SnapSkillzz aims to offer a seamless learning experience through the following key features:

### 1. Administrator Panel

Administrators have access to specific endpoints for managing courses, user information, and authentication. The administrator functionalities include:

- **Admin Authentication**: Admins can sign up and log in securely using JWT-based authentication.

- **Course Management**: Admins can create new courses, update existing course details, and retrieve information about all courses. Each course is defined by its title, description, price, image link, and publication status.

- **Admin Profile**: An endpoint allows admins to retrieve their own profile information.

### 2. User Interface

Users interact with the platform primarily through user-specific endpoints that focus on account creation, course discovery, and course purchasing. User-specific functionalities include:

- **User Authentication**: Users can sign up and log in securely using JWT-based authentication.

- **Course Discovery**: Users can retrieve a list of published courses available on the platform.

- **Course Purchase**: Users can purchase courses they are interested in, and the platform keeps track of their purchased courses.

- **Purchased Course Retrieval**: Users can view a list of courses they have previously purchased.

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/SnapSkillzz-Server.git
   cd SnapSkillzz-Server
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Set up MongoDB:**
   - Ensure MongoDB is installed and running.
   - Update the connection string in `E:\SnapSkillzz\server\index.js` with your MongoDB connection details.

4. **Run the Server:**
   ```bash
   npm start
   ```
   The server will be accessible at `http://localhost:4000`.

## How SnapSkillzz Works

1. **Admin Operations:**
   - Admins sign up and log in to the platform, gaining access to the admin panel.
   - They can create and manage courses, update course details, and retrieve information about all courses.
   - Admins can also view their own profile information.

2. **User Experience:**
   - Users sign up and log in to the platform, enabling them to explore available courses.
   - They can purchase courses they are interested in, and the system tracks their purchased courses.
   - Users can view a list of courses they have previously purchased.

## API Endpoints

Detailed information about API endpoints for administrators and users is provided in the [API Endpoints](#api-endpoints) section of the readme.

## Important Notes

- Securely manage JWT secrets, MongoDB connection details, and other sensitive information.
- This project is for educational purposes, and security considerations should be taken into account for a production environment.

## Acknowledgments

This project was created as part of a learning experience and is not intended for production use without proper security enhancements.
