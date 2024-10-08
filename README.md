

# Django-React Task Manager

This project demonstrates how to integrate a Django backend with a React frontend using Django REST Framework. The application is a simple task manager where users can create, edit, delete, and view tasks.

## Table of Contents

- [Installation](#installation)
- [Project Structure](#project-structure)
- [Features](#features)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Installation

### Prerequisites

Before running the project, ensure you have the following installed on your system:

- Python 3.x
- Node.js
- npm (Node Package Manager)
- Django

### Backend Setup (Django)

1. **Clone the Repository**

   
   git clone https://github.com/yourusername/django-react-task-manager.git
   cd django-react-task-manager
  

2. **Create a Virtual Environment**

   
   python -m venv env


3. **Activate the Virtual Environment**


     .\env\Scripts\activate
     ```
   
  
    
  

5. **Run Migrations**

   
   python manage.py migrate
  

6. **Start the Django Development Server**

   
   python manage.py runserver
   

### Frontend Setup (React)

1. **Navigate to the Frontend Directory**

   
   cd frontend
   

2. **Install Frontend Dependencies**

   
   npm install
   

3. **Start the React Development Server**

   
   npm start
   

## Project Structure

```
django-react-task-manager/
│
├── backend/                # Django project directory
│   ├── backend/            # Backend project settings
│   ├── todo/               # Task app
│   ├── db.sqlite3          # SQLite database file
│   ├── manage.py           # Django project management script
│
├── frontend/               # React frontend
│   ├── public/             # Public assets
│   ├── src/                # React source code
│   ├── package.json        # React dependencies and scripts
│
├── requirements.txt        # Backend dependencies
├── README.md               # Project documentation
```

## Features

- **Task Management**: Users can create, edit, delete, and view tasks.
- **Backend**: Django REST Framework provides a RESTful API for task management.
- **Frontend**: React handles the user interface, interacting with the Django API via Axios.

## Usage

1. **Navigate to `http://localhost:3000`** to interact with the React frontend.
2. **API Endpoints** are accessible via `http://localhost:8000/api/tasks/`.

## API Endpoints

- `GET /api/tasks/`: Retrieve all tasks.
- `POST /api/tasks/`: Create a new task.
- `PUT /api/tasks/{id}/`: Update an existing task.
- `DELETE /api/tasks/{id}/`: Delete a task.

