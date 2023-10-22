# Code Style Guide

## Python (Flask) Code Style

### Importing Libraries

- Import Flask-related libraries at the beginning of your Python file.
- Organize imports with line breaks for better readability.

### Creating a Flask Application

- Create a Flask application instance using `Flask(__name__)`.

### Handling Cross-Origin Requests

- Allow cross-origin requests using the `CORS` library if needed.
- Configure CORS for your Flask app.

### Database Connection

- Establish a connection to a MySQL database.
- Replace placeholder information (host, user, password, database) with actual database connection details.

### Handling POST Requests

- Define a route for handling POST requests.
- Access JSON data from the request using `request.get_json()`.
- Implement error handling for potential exceptions.
- Insert data into the database using SQL statements.
- Commit changes to the database.
- Close the database cursor after execution.

### Handling GET Requests

- Define a route for handling GET requests.
- Access data from the database and execute a SELECT SQL query.
- Transform query results into JSON format.
- Implement error handling for potential exceptions.

### Running the Flask App

- Launch the Flask application when the script is executed directly.

```python
if __name__ == '__main__':
    app.run(host='localhost', port=5000)
