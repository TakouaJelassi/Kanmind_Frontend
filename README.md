# Kanmind Frontend

Vanilla JavaScript frontend for Kanmind, a Kanban-style task management app. It connects to the separate Django REST API and provides authentication, dashboards, boards, tasks, assignments, and comments.

## Tech Stack

- HTML
- CSS
- Vanilla JavaScript
- Local font and icon assets
- Browser `fetch` API

## Getting Started

### 1. Start the backend

Run the Kanmind backend locally at:

```text
http://127.0.0.1:8000/api/
```

### 2. Start the frontend

Open this project with a static web server, for example the VS Code Live Server extension.

Start from the root `index.html`. The app redirects authenticated users to the dashboard and unauthenticated users to the login page.

## API Configuration

The API base URL is configured in `shared/js/config.js`.

- Localhost: `http://127.0.0.1:8000/api/`
- Production: `https://kanmind-backend-rtam.onrender.com/api/`

Adjust `PRODUCTION_API_BASE_URL` when deploying your own backend.

## Project Structure

```text
Kanmind_Frontend/
├── assets/       # Fonts, icons, and images
├── pages/        # Auth, dashboard, boards, board detail, legal pages
├── shared/       # Shared CSS and JavaScript utilities
├── index.html    # App entry redirect
└── README.md
```

## Portfolio Notes

This repository is intentionally framework-free to demonstrate DOM work, modular JavaScript helpers, API integration, and responsive CSS without a build step.
