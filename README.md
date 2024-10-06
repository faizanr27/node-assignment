# Node js Assignment

A simple RESTful API built with Express.js and MongoDB for managing items (CRUD operations). This API allows you to create, read, update, and delete items.

## Features

- Create an item
- Retrieve all items
- Update an item by ID
- Delete an item by ID

## Technologies

- Node.js
- Express.js
- MongoDB with Mongoose
- dotenv for environment variables

## Getting Started

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)
- [Git](https://git-scm.com/)
- [npm](https://www.npmjs.com/)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/faizanr27/node-assignment.git
   ```
2. Navigate to the project directory:
   ```bash
   cd node-assignment
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Create a .env file in the root of your project and add your MongoDB connection string:
   ```bash
   MONGODB_URI=your-mongodb-uri
   PORT=5000
   ```
5. Run the application:
   ```bash
   npm start
   ```
 <h5>The server will run on http://localhost:5000.</h5>

## API Endpoints
| Method | Endpoint         | Description            |
|--------|------------------|------------------------|
| GET    | `/api/items`      | Get all items          |
| POST   | `/api/items`      | Create a new item      |
| PUT    | `/api/items/:id`  | Update an item by ID   |
| DELETE | `/api/items/:id`  | Delete an item by ID   |

## Example Item Object
   ```bash
   {
      "name": "Sample Item",
      "description": "This is a sample item description.",
      "price": 19.99
   }

   ```
## Folder Structure
```bash
.
├── controllers
│   └── item.controllers.js   # Controller functions for item CRUD operations
├── db
│   └── db.js                 # MongoDB connection setup
├── models
│   └── item.models.js        # Mongoose schema for item
├── routes
│   └── item.routes.js        # API routes for item CRUD operations
├── .env                      # Environment variables
├── server.js                 # Main entry point for the application
└── package.json              # Project metadata and dependencies
```
