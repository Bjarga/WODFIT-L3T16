# WODFIT Crossfit Application

## Introduction

WODFIT is a full-stack MERN application designed to help CrossFit groups and gyms manage and track their workouts and member progress. The app facilitates the creation and sharing of workouts, logging performance, and maintaining a leaderboard to motivate members.

## Features

- **User Roles:** Coach (admin) and regular users.
- **Authentication:** Secure login and registration with options for Google and Facebook login.
- **Dashboard:** Separate dashboards for coaches and users.
- **Workout Management:** Coaches can post workouts, and users can view and log their performance.
- **Leaderboard:** View and compare scores among members.
- **Gallery:** Upload and manage photos.

## How to Use the App

### Registration and Login:

- Users can register as either a coach or join an existing coach's group.
- Secure login is available via email/password, Google, or Facebook.

### Pre-configured Team:

To see how the app works, you can use the following pre-configured team and user logins:

**Team: SmashingTigers**

**Admin/Coach:**

- Email: `Coach@gmail.com`
- Password: `coach@80`

**User1:**

- Email: `jenna@gmail.com`
- Password: `jenna@007`

**User2:**

- Email: `james@gmail.com`
- Password: `james@40`

**User3:**

- Email: `jojo@gmail.com`
- Password: `joann@jo23`

**User4:**

- Email: `kevin@gmail.com`
- Password: `kev80man`

**User5:**

- Email: `sarah@gmail.com`
- Password: `sarah@30ish`

### Dashboard:

     Coaches have access to a coach dashboard where they can manage workouts, view team profiles, and manage the gallery.
    Users have access to a user dashboard where they can view and log workouts, update their profile, and see the leaderboard.

### Workouts:

    Coaches can create, edit, and delete workouts.
    Users can view workouts and log their performance, which will be reflected on the leaderboard.

### Gallery:

    Both coaches and users can upload photos to the gallery.
    Coaches can delete photos from the gallery.

## Installation and Setup:

### Repository:

    github https://github.com/Bjarga/WODFIT-app
    cd wodfit

## Install Dependencies:

    Run the following command from the root directory to install all dependencies:
    npm install

## Environment Variables:

    Create a .env file in both the backend and client directories and configure the following variables:

# Backend (.env):

    PORT=5000
    MONGO_URI=your_mongodb_uri
    JWT_SECRET=your_jwt_secret

# Client (.env):

    REACT_APP_API_URL=http://localhost:5000

## Running the Application:

    Start the application using the following command:
    npm start
    This will concurrently start both the backend and frontend servers.

### Security Measures

- **Environment Variables:** Sensitive information like API keys and database URIs are stored in environment variables.
- **Authentication:** User authentication is handled using JWT tokens.
- **Secure Storage:** Passwords are hashed before storing in the database.

### Third-Party APIs

    Google and Facebook Authentication: Integrated for seamless user login using Passport.js with passport-google-oauth20 and passport-facebook.

### Deployment

- **Deployment Details:** The application is deployed on Vercel.
- **Deployment Structure:** The backend and frontend are deployed separately for better scalability and maintainability.

### Links

Deployed Application: WODFIT App
