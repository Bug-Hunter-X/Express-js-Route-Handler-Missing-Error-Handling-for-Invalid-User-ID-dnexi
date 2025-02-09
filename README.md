# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  lack of error handling for invalid input. Specifically, this example shows a route that retrieves a user by ID, but fails to handle cases where the ID is not a valid integer.

The `bug.js` file contains the flawed code, while `bugSolution.js` provides a corrected version with robust error handling.

## How to reproduce the bug

1. Clone this repository.
2. Run `npm install express` to install the required dependency.
3. Run `node bug.js`. 
4. Access the route `/users/abc` in your browser or using a tool like `curl`.  The server will likely crash or produce an unexpected error.

## Solution

The `bugSolution.js` file shows the improved code, including input validation and error handling, to prevent crashes and provide a more graceful user experience.