# CRUD Project for a To-Do List

This project contains CRUD (Create, Read, Update, and Delete) operations for a to-do list in the community library.

## Features:

1. Get all tasks, status, and task assignees.
2. Get a task, status, and task assignee by its ID.
3. Create and/or add a new task or task assignee.
4. Update information of a task, status, or task assignee as needed.
5. Delete a task, status, or task assignee by its ID.

## Technologies Used:

- JavaScript
- Node.js
- Express
- MongoDB
- Mongoose
- Nodemon
- Body Parser
- EJS
- Dotenv
- HTML
- CSS

## Usage:

1. Start the application: npm start or nodemon or node index.js.
2. You can test the following endpoints from Postman, which return and receive data in JSON format.

### Endpoints for Tasks:

- Get all tasks: GET /api/todo/
- Get a task by its ID: GET /api/todo/{id}
- Create a new task: POST /api/todo/create with the following JSON structure:
  
json
  {
    "task": "Assign genres to books",
    "task_responsable": "Gabriel Garcia",
    "deadline": "06-15-2023",
    "status": "64a600bda2472a22f78cf5b8",
    "update": "Need to categorize all the books"
  }
  
- Update a task by its ID: PATCH /api/todo/update/{id} with the following JSON structure:
  
json
  {
    "task": "Organize books",
    "task_responsable": "Gabriel Garcia",
    "deadline": "06-15-2023",
    "status": "64a600bda2472a22f78cf5b8",
    "update": ""
  }
  
- Delete a task by its ID: DELETE /api/todo/delete/{id}

### Endpoints for Status:

- Get all status: GET /api/status/
- Get a status by its ID: GET /api/status/{id}
- Update a status by its ID: PATCH /api/status/update/{id} with the following JSON structure:
  
json
  {
    "status": "pending"
  }
  

### Endpoints for Task Assignees:

- Get all task assignees: GET /api/responsable/
- Get a task assignee by its ID: GET /api/responsable/{id}
- Create a new task assignee: POST /api/responsable/create with the following JSON structure:
  
json
  {
    "task_responsable": "Kevin"
  }
  
- Update a task assignee by its ID: PATCH /api/responsable/update/{id} with the following JSON structure:
  
json
  {
    "task_responsable": "Santiago"
  }
  
- Delete a task assignee by its ID: DELETE /api/responsable/delete/{id}

You can access the application and its front-end interface at http://localhost:3000/.

## About:

This project is a CRUD to-do list for the community library. It provides an API for managing tasks, status, and task assignees associated with the tasks.
