Secrets Sharing App
This is a full-stack web application that allows users to share secrets anonymously. The app uses secure user authentication to protect users' privacy and offers a simple, intuitive interface for sharing and viewing secrets.

Features
Anonymous Secret Sharing: Users can share secrets anonymously, visible only after logging in.
User Authentication: Supports secure login and registration using local credentials or Google OAuth.
Password Security: Passwords are securely hashed with bcrypt before storage.
Session Management: Sessions are managed with express-session to maintain user login state.
Technologies Used
Front End: HTML, CSS, Bootstrap, EJS templating
Back End: Node.js, Express
Database: PostgreSQL for storing user data and secrets
Authentication: Passport.js for user authentication, supporting Local and Google OAuth strategies
Environment Management: dotenv for securely handling sensitive information like API keys
Project Structure
Front-End Views: EJS templates (home.ejs, login.ejs, register.ejs, secrets.ejs, submit.ejs)
CSS Styling: Basic custom styling is included in style.css for UI enhancement
Server Setup: All server routes and configurations are managed in index.js
Getting Started
Prerequisites
Install Node.js and npm
Install PostgreSQL and set up a database
Obtain Google OAuth credentials (Client ID and Client Secret)
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/secrets-sharing-app.git
cd secrets-sharing-app
Install dependencies:

bash
Copy code
npm install
Set up environment variables in a .env file:

plaintext
Copy code
SESSION_SECRET=your_session_secret
PG_USER=your_postgres_username
PG_HOST=your_postgres_host
PG_DATABASE=your_database_name
PG_PASSWORD=your_postgres_password
PG_PORT=your_postgres_port
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
Set up the PostgreSQL database:

Create a users table with columns for email, password, and secret.
Start the server:

bash
Copy code
npm start
The application should be running on http://localhost:3000.

Usage
Register: Users can create an account by signing up with email and password or by using Google OAuth.
Login: Registered users can log in to access the secret sharing feature.
Submit a Secret: Logged-in users can submit secrets anonymously to be viewed only by other authenticated users.
Logout: Users can securely log out to end their session.
