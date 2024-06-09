# Notes Writing App

A web application that allows users to register, login, write, and delete notes. The frontend is built using React, and the backend is powered by Django.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- User registration and authentication
- Create, view, and delete notes
- Responsive UI

## Technologies Used

- **Frontend**: React, JavaScript, HTML, CSS
- **Backend**: Django, Django REST Framework
- **Database**: SQLite (default), can be changed to PostgreSQL or other databases

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js and npm installed on your machine
- Python and pip installed on your machine
- Virtualenv installed (optional but recommended)

## Installation

### Backend (Django)

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/notes-writing-app.git
   cd notes-writing-app/backend
   ```

2. Create and activate a virtual environment:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the dependencies:
   ```sh
   pip install -r requirements.txt
   ```

4. Apply the migrations:
   ```sh
   python manage.py migrate
   ```

5. Create a superuser to access the Django admin panel:
   ```sh
   python manage.py createsuperuser
   ```

6. Start the development server:
   ```sh
   python manage.py runserver
   ```

### Frontend (React)

1. Navigate to the frontend directory:
   ```sh
   cd ../frontend
   ```

2. Install the dependencies:
   ```sh
   npm install
   ```

3. Start the React development server:
   ```sh
   npm start
   ```

The React app should now be running on `http://localhost:3000` and the Django server on `http://localhost:8000`.

## Usage

1. Open your browser and navigate to `http://localhost:3000`.
2. Register a new account or login with existing credentials.
3. Create, view, and delete notes as needed.

## API Endpoints

### Authentication

- `POST /api/auth/register/` - Register a new user
- `POST /api/auth/login/` - Login a user and obtain a token
- `POST /api/auth/logout/` - Logout a user

### Notes

- `GET /api/notes/` - Retrieve all notes for the logged-in user
- `POST /api/notes/` - Create a new note
- `DELETE /api/notes/:id/` - Delete a note by ID

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

1. Fork the Project
2. Create your Feature Branch 
3. Commit your Changes
4. Push to the Branch
5. Open a Pull Request
