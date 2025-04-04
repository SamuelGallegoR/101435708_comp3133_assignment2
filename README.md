# Employee Management App

A full-stack employee management system built with **Angular (Standalone Components)** on the frontend and a **GraphQL API** backend. This app allows users to add, view, search, and delete employees with real-time updates and a clean UI.

---

## ✨ Features

- 🔍 Search employees by **name**, **email**, or **designation**
- ➕ Add new employees with **form validation**
- 🗑️ Delete employees with **confirmation prompts**
- 🖼️ Live **photo URL preview** in the form
- 🔄 Auto-refresh of employee list after adding or deleting entries

---

## 🛠️ Tech Stack

### Frontend
- Angular 16+ (Standalone Components)
- Reactive Forms
- Angular Router

### Backend (in Docker)
- Node.js with GraphQL server
- PostgreSQL database
- Docker + Docker Compose

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/employee-management-app.git
cd employee-management-app
```

### 2. Start Backend (GraphQL + Postgres) via Docker

```bash
docker-compose up --build
```

> Ensure Docker is installed and running on your machine.

### 3. Start Angular Frontend

```bash
cd frontend
npm install
ng serve
```

Navigate to: [http://localhost:4200](http://localhost:4200)

---

## 📁 Project Structure

```
employee-management-app/
│
├── frontend/
│   └── src/app/
│       ├── services/graphql.service.ts     # Handles GraphQL API calls
│       ├── employee-add/                   # Component to add employees
│       ├── employee-list/                  # Component to list, search, and delete employees
│       └── shared/navbar/                  # Navbar component
│
├── backend/
│   ├── server.js                           # GraphQL server entry
│   └── docker-compose.yml                  # Backend container setup
```

---

## ⚙️ Environment Variables

In the backend project, configure environment variables (e.g., DB URL, port) in a `.env` file or directly inside `docker-compose.yml`.

---

## 📦 Example Employee Object

```json
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
```

---

## 👥 Contributors

- **Samuel Gallego Rivera** – Frontend & Architecture  
- [Add your teammates here]

---

## 🔮 Future Improvements

- GraphQL mutation for **update** operations
- Individual **profile view** per employee
- **Image upload** functionality instead of URL input
- **Role-based access control**

---

## 📝 License

🪲 Beetle Labs Inc. 🍋‍🟩 GreenConcept LLC.
