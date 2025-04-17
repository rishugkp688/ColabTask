# CollabTask - Real-time Collaborative Task Manager

## Description

CollabTask is a real-time collaborative task management platform designed to help teams stay organized and productive. It allows users to create, assign, and track tasks seamlessly, with updates reflected instantly across all connected users thanks to WebSocket technology.

The frontend leverages the power of HTMX and Alpine.js for a dynamic and responsive user experience without complex JavaScript frameworks. The backend is built with Go, providing performance and efficiency, while PostgreSQL serves as the robust database solution. Secure user sessions are managed using JWT authentication.

## ✨ Features

* **Real-time Collaboration:** See updates from teammates instantly without refreshing the page.
* **Task Management:** Create, view, update, and delete tasks.
* **Task Assignment:** Assign tasks to specific team members.
* **Status Tracking:** Monitor the progress of tasks (e.g., To Do, In Progress, Done).
* **User Authentication:** Secure login and session management using JWT.
* **Dynamic UI:** Interactive user interface powered by HTMX and Alpine.js.
* **RESTful API:** Well-defined API endpoints for communication between frontend and backend.

## 🚀 Tech Stack

* **Backend:** Go
* **Frontend:** HTMX, Alpine.js, HTML, CSS (Consider adding Tailwind CSS if used)
* **Database:** PostgreSQL
* **Real-time Communication:** WebSocket
* **Authentication:** JWT (JSON Web Tokens)
* **API:** RESTful

## ⚙️ Getting Started

### Prerequisites

* Go (Version X.X.X or higher)
* PostgreSQL (Version X.X or higher)
* Node.js & npm (Optional, if using a build process for frontend assets)
* Git

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/collabtask.git](https://github.com/your-username/collabtask.git)
    cd collabtask
    ```

2.  **Backend Setup:**
    * Navigate to the backend directory (`cd backend` - adjust path if needed).
    * Configure database connection details (e.g., in a `.env` file or config file). Example `.env`:
        ```
        DB_HOST=localhost
        DB_PORT=5432
        DB_USER=your_db_user
        DB_PASSWORD=your_db_password
        DB_NAME=collabtask_db
        JWT_SECRET=your_very_secret_key
        ```
    * Run database migrations (if applicable).
        ```bash
        # Add command for running migrations
        ```
    * Install Go dependencies:
        ```bash
        go mod tidy
        ```
    * Build the backend:
        ```bash
        go build -o main .
        ```
    * Run the backend server:
        ```bash
        ./main
        # Or: go run main.go
        ```

3.  **Frontend Setup:**
    * The frontend primarily uses static files served by the Go backend or a separate web server.
    * Ensure HTML files correctly link to HTMX and Alpine.js (usually via CDN or local files).
    * If using npm for asset management (e.g., Tailwind CSS):
        ```bash
        # cd frontend (adjust path if needed)
        # npm install
        # npm run build (or watch)
        ```

4.  **Database Setup:**
    * Create a PostgreSQL database named `collabtask_db` (or as configured).
    * Create the necessary tables (provide schema or migration commands).

### Accessing the Application

Open your web browser and navigate to `http://localhost:PORT` (replace `PORT` with the port your Go application is running on, e.g., 8080).

## 📖 Usage

1.  **Register/Login:** Create a new account or log in with existing credentials.
2.  **Dashboard:** View your assigned tasks and project boards.
3.  **Create Task:** Click the "New Task" button, fill in the details (title, description, assignee, due date), and save.
4.  **Update Task:** Drag and drop tasks between columns (e.g., To Do, In Progress, Done) or click on a task to edit its details.
5.  **Real-time Updates:** Changes made by you or other users will appear automatically.

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/your-feature-name`).
3.  Make your changes.
4.  Commit your changes (`git commit -m 'Add some feature'`).
5.  Push to the branch (`git push origin feature/your-feature-name`).
6.  Open a Pull Request.

Please ensure your code adheres to the project's coding standards and includes tests where applicable.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. ( **Note:** You'll need to create a `LICENSE` file, typically containing the MIT License text).

---

_Happy Collaborating!_
