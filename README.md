# evel

A minimal Express server with a health endpoint.

## Setup

```bash
npm install
```

## Usage

```bash
npm start
```

Server runs on port 3000 by default. Set the `PORT` environment variable to override.

## Endpoints

| Method | Path | Response |
|--------|------|----------|
| GET | `/health` | `{"status":"ok"}` |
| POST | `/echo` | Echoes the request body as JSON |

## Development

All commits are managed by the `code-commiter` Claude Code agent using the [Conventional Commits](https://www.conventionalcommits.org) specification.
