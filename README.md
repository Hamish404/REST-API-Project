# Secrets API Client

This repository contains a simple client built with Express.js, Axios, and EJS that interacts with the Secrets API (https://secrets-api.appbrewery.com).  It demonstrates how to perform CRUD (Create, Read, Update, Delete) operations using various HTTP methods.

## Features

*   **GET /secrets/{id}:** Retrieves a secret by its ID.
*   **POST /secrets:** Creates a new secret.
*   **PUT /secrets/{id}:** Updates an existing secret completely.
*   **PATCH /secrets/{id}:** Partially updates an existing secret.
*   **DELETE /secrets/{id}:** Deletes a secret.
*   
*   **Bearer token authentication:**  Securely authenticates requests using a bearer token.
*   **EJS templating:**  Uses EJS for dynamic HTML rendering.
*   **Axios for HTTP requests:**  Simplifies making HTTP requests to the Secrets API.

## Technologies Used

*   **Node.js:** JavaScript runtime environment.
*   **Express.js:** Web application framework for Node.js.
*   **Axios:** HTTP client for making requests to external APIs.
*   **EJS (Embedded JavaScript):** Templating engine for generating HTML.
*   **Body-parser:** Middleware for parsing request bodies.

## Installation

1.  Clone the repository:

    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://www.google.com/search?q=https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
    ```

2.  Navigate to the project directory:

    ```bash
    cd YOUR_REPO_NAME
    ```

3.  Install dependencies:

    ```bash
    npm install
    ```

## Usage

1.  **Set your Bearer token:** Replace `"0c60888b-20bb-4352-9952-3c56fe9ba92e"` in `index.js` with your actual Bearer token.  You can obtain a bearer token from the API provider.

2.  Start the server:

    ```bash
    node index.js
    ```

3.  Open your browser and go to `http://localhost:3000`.

4.  Use the form to interact with the Secrets API:
    *   Enter the `id`, `secret`, and `score` (if applicable).
    *   Click the appropriate button (GET, POST, PUT, PATCH, DELETE) to send the request to the API.
    *   The response from the API will be displayed on the page.

## API Documentation

Refer to the official Secrets API documentation for details on the available endpoints and request/response formats: https://secrets-api.appbrewery.com

## Important Considerations

*   **Bearer Token Security:**  Do not expose your Bearer token in client-side code or commit it to version control.  In a production environment, you would typically store the token securely on the server and not include it directly in the client-side code. This is for demonstration purposes only.
*   **Error Handling:**  The code includes basic error handling, but you might want to add more robust error handling for a production application.
*   **Input Validation:**  It's recommended to add input validation to your forms to prevent invalid data from being sent to the API.
