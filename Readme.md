# Development Guide

## Prerequisites

- Node.js (v16+)
- Docker
- Git

## Setup

1. Clone the repository.
2. Install dependencies: `npm install`
3. Set up environment: `cp .env.example .env` and edit.
4. Start the database: `docker-compose up -d`
5. Run migrations: `npm run migrate`
6. Start the development server: `npm run dev`

## Testing

- `npm test` for unit tests.
- `npm run test:e2e` for end-to-end tests.

## Code Style

- ESLint for linting.
- Prettier for formatting.

## Technologies

- **React**: A JavaScript library for building user interfaces.
- **Express**: Fast, unopinionated, minimalist web framework for Node.js.
- **PostgreSQL**: A powerful, open source object-relational database.
- **Docker**: A platform for developing, shipping, and running applications in containers.
- **Git**: Distributed version control system.