1. GitHub README File
markdown
Copy
Edit
# File Storage App

A simple file storage application built with [Node.js](https://nodejs.org/), [Express](https://expressjs.com/), [Multer](https://github.com/expressjs/multer), and [EJS](https://ejs.co/). This app allows users to upload files, view them with custom icons based on file type, and delete files from the server. It's a great starting point for learning file management in a Node.js environment.

## Features

- **File Upload:** Upload files using a simple form powered by Multer.
- **File Listing:** View all uploaded files with icons representing file types (PDF, Word, Excel, images, etc.).
- **File Deletion:** Remove unwanted files from the storage directory.
- **Static File Serving:** Access uploaded files directly through a public URL.
- **Templating:** Render views using EJS and style them with Bootstrap.

## Prerequisites

- [Node.js](https://nodejs.org/) (v12 or later)
- npm (comes with Node.js)

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/file-storage-app.git
   cd file-storage-app

Access the app:

Open your browser and navigate to http://localhost:3000.

Upload, view, and delete files:

Use the "Upload File" form to add new files.
See a list of uploaded files along with icons that represent their type.
Delete files using the provided dropdown menu.
API Endpoints
GET /
Renders the main page (index view).

POST /upload
Endpoint for uploading a file. Accepts a file via form data (key: file).

GET /view
Returns a JSON object containing the list of files in the filestorage directory.

DELETE /delete/:fileName
Deletes the specified file from the server.

