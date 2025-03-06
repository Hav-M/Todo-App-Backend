# Todo App Backend

This is the backend for a simple Todo App built using **Node.js, Express, MySQL, and JWT Authentication**. The backend provides APIs for user authentication, adding, updating, retrieving, and deleting todos.

## Features
- User Registration & Login with password hashing using **bcryptjs**
- JWT-based authentication
- CRUD operations for todos
- MySQL database integration

## Technologies Used
- **Node.js**
- **Express.js**
- **MySQL2**
- **bcryptjs** (for password hashing)
- **jsonwebtoken** (for authentication)
- **dotenv** (for environment variables)
- **cors** (for cross-origin support)

## Setup Instructions

### 1. Clone the Repository
```
git clone https://github.com/yourusername/todo-app-backend.git
cd todo-app-backend
```

### 2. Install Dependencies
```
npm install
```

### 3. Setup Environment Variables
Create a `.env` file in the root directory and add your database credentials:
```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=yourpassword
DB_NAME=todo_app
SECRET_KEY=your_secret_key
```

### 4. Start the Server
```
node server.js
```
The server will run on `http://localhost:5000`

## API Endpoints

### Authentication
- **POST /api/register** – Register a new user
- **POST /api/login** – Login and get a JWT token

### Todos
- **GET /api/todos** – Fetch all todos (requires authentication)
- **POST /api/todos** – Add a new todo (requires authentication)
- **PUT /api/todos/:id** – Update a todo (requires authentication)
- **DELETE /api/todos/:id** – Delete a todo (requires authentication)

## Contributing
Feel free to submit issues or pull requests.

## License
This project is licensed under the MIT License.

---
### Author
[Your Name](https://github.com/yourusername)

