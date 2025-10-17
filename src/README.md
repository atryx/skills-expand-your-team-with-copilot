# Mergington High School Activities

A web application that allows students to explore extracurricular activities and enables teachers to manage student registrations.

## Features

### For Students
- **Browse Activities**: View all available extracurricular activities with detailed information including:
  - Activity description
  - Schedule (days and times)
  - Maximum capacity
  - Current enrollment
- **Advanced Filtering**: Filter activities by:
  - Category (Sports, Arts, Academic, Community, Technology)
  - Day of the week (Monday through Sunday)
  - Time of day (Before School, After School, Weekend)
- **Search**: Search activities by name or description
- **View Schedules**: See detailed schedule information including days and times for each activity

### For Teachers
- **Secure Login**: Teachers can log in with their credentials to manage student registrations
- **Register Students**: Add students to activities using their email addresses
- **Unregister Students**: Remove students from activities when needed
- **Session Management**: Persistent login sessions for convenience

## Technology Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python with FastAPI framework
- **Database**: MongoDB for persistent data storage
- **API**: RESTful API with multiple endpoints for activities and authentication

## API Endpoints

- `GET /activities` - Get all activities with optional filtering by day and time
- `GET /activities/days` - Get a list of all days that have activities scheduled
- `POST /activities/{activity_name}/signup` - Register a student for an activity (requires teacher authentication)
- `POST /activities/{activity_name}/unregister` - Remove a student from an activity (requires teacher authentication)
- `POST /auth/login` - Teacher login
- `GET /auth/check-session` - Check if a teacher session is valid

## Development Guide

For detailed setup and development instructions, please refer to our [Development Guide](../docs/how-to-develop.md).
