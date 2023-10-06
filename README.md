# TestnezhadCRM

This repository contains a simple frontend application that demonstrates how to communicate with a backend API.

The project is designed for educational purposes and aims to showcase how a frontend can interact with an API to perform basic CRUD operations.

## Project Description

The frontend application is built using three HTML files: create.html, edit.html, and index.html. These files allow you to create, edit, delete, and list imaginary users, similar to a simple address book. Each user entry consists of a first name, last name, and mobile number.

## Installation and Setup

To run the project, you have two options:

### Option 1: Running in the Browser

1. Clone this repository to your local machine:

```bash
git clone https://github.com/TheWation/TestnezhadCRM
```

```bash
cd TestnezhadCRM/dist
```

Open any of the HTML files (create.html, edit.html, index.html) in your preferred web browser.

### Option 2: Running with Python's http.server module

1. Ensure you have Python installed on your system.

2. Clone this repository to your local machine:

```bash
git clone https://github.com/TheWation/TestnezhadCRM
```


3. Navigate to the project directory:

```bash
cd TestnezhadCRM/dist
```

4. Start a simple HTTP server using Python's http.server module:

```bash
python -m http.server
```

This will start the server on `http://localhost:8000`.

Open your preferred web browser and access the application using the appropriate URL:

- List Users: http://localhost:8000/index.html
- Create User: http://localhost:8000/create.html
- Edit User: http://localhost:8000/edit.html

## Backend Considerations
If you want to create a backend for this frontend, it's important to note that if the origin of the frontend and backend are not the same, you need to allow Cross-Origin Resource Sharing (CORS) for the frontend origin.

The required endpoints for this frontend to work are:


- `GET` /users: This endpoint returns a JSON list of users.
- `POST` /users: This endpoint creates a user by accepting a JSON object containing the firstname, lastname, and mobile fields.
- `GET` /users/{user_id}: This endpoint retrieves user data based on the provided user_id and returns it as a JSON object.
- `PUT` /users/{user_id}: This endpoint updates user information by accepting a JSON object containing the firstname, lastname, and mobile fields.
- `DELETE` /users/{user_id}: This endpoint deletes the user with the provided user_id.

Please ensure that your backend API implements these endpoints and handles the necessary CRUD operations accordingly.

## Contributing

Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

## Disclaimer
Please note that this project is intended for educational purposes only. It is a basic demonstration of frontend API communication and may not adhere to best practices or cover all aspects of a production-ready application.