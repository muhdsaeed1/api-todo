# ToDo Backend API using Node.js and Express

This is a simple ToDo backend API built with Node.js and Express. It provides basic CRUD (Create, Read, Update, Delete) operations for managing ToDo items.

## Getting Started

Follow the instructions below to set up and run the ToDo backend API on your local machine.

### Prerequisites

- Node.js: Make sure you have Node.js installed. You can download it [here](https://nodejs.org/).

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/todo-backend-node-express.git
   ```

2. Navigate to the project directory:

   ```bash
   cd todo-backend-node-express
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

### Configuration

Create a `.env` file in the root of the project and configure the following variables:

```env
PORT=3000
MONGODB_URI=mongodb://localhost:27017/todo
```

Adjust the values according to your preferences and MongoDB setup.

### Running the Application

Start the application with the following command:

```bash
npm start
```

The API will be accessible at `http://localhost:3000` by default.

## API Endpoints

### 1. Get All ToDo Items

- **Endpoint**: `GET /todos`
- **Description**: Retrieve all ToDo items.
- **Example**: `http://localhost:3000/todos`

### 2. Get a ToDo Item by ID

- **Endpoint**: `GET /todos/:id`
- **Description**: Retrieve a ToDo item by its ID.
- **Example**: `http://localhost:3000/todos/1`

### 3. Create a ToDo Item

- **Endpoint**: `POST /todos`
- **Description**: Create a new ToDo item.
- **Example**: `http://localhost:3000/todos`
- **Request Body**:
  ```json
  {
    "title": "Complete Project",
    "completed": false
  }
  ```

### 4. Update a ToDo Item

- **Endpoint**: `PUT /todos/:id`
- **Description**: Update a ToDo item by its ID.
- **Example**: `http://localhost:3000/todos/1`
- **Request Body**:
  ```json
  {
    "completed": true
  }
  ```

### 5. Delete a ToDo Item

- **Endpoint**: `DELETE /todos/:id`
- **Description**: Delete a ToDo item by its ID.
- **Example**: `http://localhost:3000/todos/1`

## Technologies Used

- Node.js
- Express
- MongoDB (Mongoose)

