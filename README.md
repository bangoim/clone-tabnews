# TabNews Clone

A full-stack clone of [TabNews](https://www.tabnews.com.br/) built with Next.js and PostgreSQL, following the [curso.dev](https://www.curso.dev/) curriculum by Filipe Deschamps.

## Motivation

I built this project to deepen my understanding of full-stack web development by following Filipe Deschamps' curso.dev. Rather than relying on tutorials that gloss over infrastructure, this course walks through building a real-world application from scratch — including database setup, API design, testing, and Docker-based development workflows. Each piece of the stack is intentional and hands-on, which is exactly the kind of learning I was looking for.

## Quick Start

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS Hydrogen)
- [Docker](https://www.docker.com/) and Docker Compose

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/clone-tab-news.git
cd clone-tab-news
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start the development server

```bash
npm run dev
```

This starts PostgreSQL via Docker Compose and launches the Next.js dev server at [http://localhost:3000](http://localhost:3000).

## Usage

### API

**`GET /api/v1/status`** — Returns the current status of the application and database connectivity.

```bash
curl http://localhost:3000/api/v1/status
```

### Available Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start database and Next.js dev server |
| `npm test` | Run the test suite |
| `npm run test:watch` | Run tests in watch mode |
| `npm run lint:check` | Check code formatting with Prettier |
| `npm run lint:fix` | Auto-fix formatting issues |
| `npm run services:up` | Start Docker services only |
| `npm run services:stop` | Stop Docker services |
| `npm run services:down` | Stop and remove Docker containers |

### Environment Variables

Defaults are provided in `.env.development`:

| Variable | Default |
| --- | --- |
| `POSTGRES_HOST` | `localhost` |
| `POSTGRES_PORT` | `5432` |
| `POSTGRES_USER` | `local_user` |
| `POSTGRES_DB` | `local_db` |
| `POSTGRES_PASSWORD` | `local_password` |

## Contributing

### Clone the repo

```bash
git clone https://github.com/<your-username>/clone-tab-news.git
cd clone-tab-news
```

### Install dependencies

```bash
npm install
```

### Start the development environment

```bash
npm run dev
```

### Run the test suite

```bash
npm test
```

### Check code formatting

```bash
npm run lint:check
```

### Submit a pull request

If you'd like to contribute, please fork the repository and open a pull request to the `main` branch.
