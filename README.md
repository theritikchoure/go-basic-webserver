# Simple GoLang Web Server

This repository contains a basic GoLang web server that serves static files and handles HTTP requests for a "hello" endpoint and a form submission.

## Table of Contents
Prerequisites
Getting Started
Endpoints
Usage
License

## Prerequisites
Before you begin, make sure you have the following installed on your system:

- [Go](https://golang.org/doc/install) (Go Programming Language)
- A web browser or a tool like [curl](https://curl.se/) to interact with the server

## Getting Started

1. Clone this repository or download the source code.
    ```powershell
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Compile and run the Go application.
    ```powershell
    go run main.go
    ```

This will start the server on port 8080.

## Endpoints

### Static Files
Static files are served from the `static` directory. You can place your HTML, CSS, JavaScript, and other static assets in this directory, and the server will serve them at the root URL.

For example, if you have an HTML file named `index.html` inside the `static` directory, you can access it at http://localhost:8080/index.html.

### Hello Endpoint
The `/hello` endpoint responds to HTTP GET requests with a simple "hello" message.

- **URL:** `/hello`
- **Method:** GET
- **Response:** "hello"

### Form Endpoint
The `/form` endpoint handles HTTP POST requests with form data. It parses the form data and displays it in the response.

- **URL:** `/form`
- **Method:** POST
- **Request Body:** Form data (e.g., `name` and `address`)
- **Response:** Displays the submitted form data.

## Usage

1. Open a web browser or use a tool like `curl` to interact with the server's endpoints.

    - Access static files by navigating to http://localhost:8080/ followed by the filename you want to access (e.g., http://localhost:8080/index.html).

    - Access the "hello" endpoint at http://localhost:8080/hello using a GET request.

    - Submit form data to the /form endpoint using a POST request and observe the response.

2. Experiment with the provided endpoints and customize the static files and server behavior as needed for your project.

## License
This project is licensed under the MIT License - see the [LICENSE]() file for details