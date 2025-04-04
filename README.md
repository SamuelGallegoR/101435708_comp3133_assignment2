Employee Management App

This is a full-stack employee management system built with Angular (Standalone Components) on the frontend and a GraphQL API backend. It allows users to add, view, search, and delete employees with real-time data updates.

Features

- Search employees by name, email, or designation
- Add new employees with form validation
- Delete employees with confirmation
- Live photo URL preview in the form
- Auto-refresh employee list after adding or deleting

Tech Stack

Frontend
- Angular 16+ (with standalone components)
- Reactive Forms
- Angular Router

Backend (in Docker)
- Node.js with GraphQL server
- PostgreSQL database
- Docker + Docker Compose

Getting Started

1. Clone the Repository
    git clone https://github.com/yourusername/employee-management-app.git
    cd employee-management-app

2. Start Backend (GraphQL + Postgres) via Docker
    docker-compose up --build
    > Make sure Docker is installed and running on your machine.

3. Start Angular Frontend
    cd frontend
    npm install
    ng serve
    Navigate to: http://localhost:4200

Project Structure

frontend/
  └── src/
      ├── app/
      │   ├── services/graphql.service.ts      # GraphQL API calls
      │   ├── employee-add/                    # Add employee form
      │   ├── employee-list/                   # List/search/delete employees
      │   └── shared/navbar/                   # Navbar component
backend/
  ├── server.js                                # GraphQL server entry
  └── docker-compose.yml                       # Backend container setup

Environment Variables

In the backend project, make sure to configure your environment variables (e.g., database URL, port) either in .env or directly in docker-compose.yml.

Example Employee Object

{
  "first_name": "Jane",
  "last_name": "Doe",
  "email": "jane.doe@example.com",
  "gender": "Female",
  "designation": "Software Engineer",
  "salary": 85000,
  "department": "Development",
  "date_of_joining": "2024-02-15",
  "employee_photo": "https://example.com/photo.jpg"
}

Contributors

- Samuel Gallego Rivera – Frontend & Architecture
- [Add your team members here]

Future Improvements

- GraphQL mutations for update operations
- Profile view per employee
- Image upload instead of URL field
- Role-based access control

License

MIT