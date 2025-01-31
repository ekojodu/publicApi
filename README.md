# Project Name: API to Fetch Current Datetime

## Description
This project provides a simple API built with [Node.js](https://hng.tech/hire/nodejs-developers) that returns the current date and time in ISO 8601 format (UTC). The API responds to GET requests with a JSON object containing the current datetime, your email, and a link to your GitHub repository. The project is designed using the Express framework, with Cross-Origin Resource Sharing (CORS) enabled.

## Features
- Dynamic generation of current date and time in ISO 8601 format (UTC).
- Supports GET requests.
- CORS support to enable cross-origin requests.
- Includes basic project metadata like email and GitHub URL in the response.
- Provides appropriate HTTP status codes for success and failure.

## Setup Instructions

### Prerequisites
- [Node.js](https://nodejs.org/) - Ensure Node.js is installed on your system.
- [npm](https://www.npmjs.com/) - Node package manager, comes installed with Node.js.

### Steps to Run the Project Locally
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/ekojodu/publicApi.git
   ```
2. Navigate to the project directory:
   ```bash
   cd publicApi
   ```
3. Install the required dependencies:
   ```bash
   npm install
   ```
4. Start the application:
   ```bash
   npm start
   ```
   By default, the server will start on [http://localhost:3000](http://localhost:3000).

5. The API should now be running locally. You can test it using a tool like [Postman](https://www.postman.com/) or cURL.

## API Documentation

### Endpoint URL
- **GET** `/`

### Request Format
- **Method**: GET
- **URL**: `/`

### Response Format
```json
{
  "email": "deblaiseuk@gmail.com",
  "current_datetime": "2025-01-31T12:34:56Z",
  "github_url": "https://github.com/ekojodu/publicApi"
}
```

- `email`: Your email address.
- `current_datetime`: The current date and time in ISO 8601 format (UTC).
- `github_url`: A link to your GitHub repository.

### Example Usage
#### Request
```bash
curl -X GET http://localhost:3000/
```

#### Response
```json
{
  "email": "deblaiseuk@gmail.com",
  "current_datetime": "2025-01-31T12:34:56Z",
  "github_url": "https://github.com/ekojodu/publicApi"
}
```

### HTTP Status Codes
- **200 OK**: The request was successful, and the datetime was returned.
- **500 Internal Server Error**: A server error occurred while processing the request.

## Code Quality
The code is organized in a straightforward manner:
- **Express** is used to handle HTTP requests.
- **CORS** is enabled to allow cross-origin requests.
- The logic is simple, focusing on responding to a single GET request with JSON data.

