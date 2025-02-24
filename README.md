# project-managing

## Overview

This project is a Proof of Concept (PoC) for a Gantt Chart application that allows users to create and manage project schedules with dependencies. The frontend is built with React.js, the backend with Python, and SQLite is used as the database.

## Features

### Frontend

- A **task panel** on the left side to enter and edit tasks
* Task name
* Start date
* End date
* Estimated duration
* Dependencies (e.g., "Task B starts after Task A is completed")
- A **Gantt Chart** on the right side that dynamically updates based on the task panel data

### Backend

- API to **add, edit, delete, and retrieve tasks**
- Automatic **schedule recalculation** based on dependencies
- **Task shifting** when dependencies change (e.g., if a task is delayed, dependent tasks adjust accordingly)

## Tech Stack

- **Frontend:** React.js
- **Backend:** Python (FastAPI or Flask recommended)
- **Database:** SQLite (for simplicity)
- **Development Environment:* GitHub Codespaces

## Installation & Setup

**1. Clone the repository**

git clone https://github.com/your-username/gantt-chart-poc.git
cd gantt-chart-poc

**2. Set up the backend**

cd backend
python -m venv venv
source venv/bin/activate  # On Windows use 'venv\Scripts\activate'
pip install -r requirements.txt
python app.py  # Start the backend server

**3. Set up the frontend**

cd frontend
npm install
npm start  # Start the frontend server

**4. Open the application**

Go to http://localhost:3000 in your browser.

## API Endpoints

- `GET /tasks` – Retrieve all tasks
- `POST /tasks` – Add a new task
- `PUT /tasks/{id}` – Edit an existing task
- `DELETE /tasks/{id}` – Remove a task

## Future Improvements

- **User authentication** (e.g., login system)
- **Drag-and-drop support** for tasks in the Gantt chart
- **Export functionality** (CSV, PDF, or JSON)


## Contributors

- **Robert (Project Owner & Developer)**
