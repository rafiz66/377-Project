# Developer Manual — BookTrack

## Overview
BookTrack is a full-stack web application built with a JavaScript-based front end and a Node.js backend. The backend exposes a REST API that communicates with a Supabase PostgreSQL database. The front end consumes all data using the Fetch API and renders content dynamically in the browser.

This document provides instructions for setting up, running, and extending the application.

## Technology Stack
- Front End: HTML, CSS, JavaScript
- Backend: Node.js (Vercel Serverless Functions)
- Database: Supabase (PostgreSQL)
- Deployment: Vercel

## Installation and Setup

### Clone the repository
```bash
git clone <your-github-repo-url>
cd booktrack
Install dependencies
bash
Copy code
npm install
Database setup
Create a Supabase project and database table.

Environment variables
Create a .env file and add:

bash
Copy code
SUPABASE_URL=your_supabase_url
SUPABASE_ANON_KEY=your_supabase_anon_key
Run the application
bash
Copy code
npm run dev
The application will be available at:

arduino
Copy code
http://localhost:3000
API Documentation
GET /api/books
Retrieves all books from the database.

Optional query parameter:

genre — filters books by genre

POST /api/books
Adds a new book to the database.

Request body fields:

title

author

genre

published_year

Known Issues
No user authentication is implemented

Input validation is minimal

Error handling is basic and can be improved

Future Development
Add user authentication and roles

Improve form validation and error handling

Add search and sorting features

Expand analytcs visualizations
