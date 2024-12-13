
# Flask Todo App

This is a simple Todo application built using Flask and SQLAlchemy. It allows users to add, update, and delete tasks.

## Features

- **Add Todos**: Create new tasks with a title.
- **Update Todos**: Mark tasks as complete or incomplete.
- **Delete Todos**: Remove tasks from the list.
- **Persistent Storage**: Uses SQLite for data storage.

## Prerequisites

- Python 3.x
- Flask
- Flask-SQLAlchemy

## Setup Instructions

1. Clone the repository or copy the code.
2. Navigate to the project directory.
3. Create a virtual environment and activate it:

   ```bash
   python -m venv myenv
   source myenv/bin/activate  # On Windows: myenv\Scripts\activate
   ```

4. Install dependencies:

   ```bash
   pip install flask flask-sqlalchemy
   ```

5. Run the application:

   ```bash
   python app.py
   ```

6. Open your browser and go to `http://127.0.0.1:5000`.

## Application Routes

- **`/`**: Displays the list of todos.
- **`/add`**: Adds a new todo (POST method).
- **`/update/<int:todo_id>`**: Toggles the completion status of a todo.
- **`/delete/<int:todo_id>`**: Deletes a todo.

## Directory Structure

```
project/
│
├── app.py          # Main application file
├── templates/
│   └── base.html   # HTML template for the app
└── db.sqlite       # SQLite database (auto-created on first run)
```

## Database Model

- **`Todo`**:
  - `id`: Integer (Primary Key)
  - `title`: String (100 characters max)
  - `complete`: Boolean (Task completion status)

## Example Usage

1. Navigate to the app in your browser.
2. Add a new task using the input form.
3. Toggle the completion status of a task using the "Update" button.
4. Remove a task using the "Delete" button.

## License

This project is free to use and modify. No license restrictions.
