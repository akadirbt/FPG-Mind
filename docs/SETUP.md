# Setup

## Overview

The project uses a Python backend and a JavaScript frontend.

Typical local workflow:

1. Create a Python virtual environment.
2. Install backend dependencies.
3. Install frontend dependencies.
4. configure local environment variables in non-committed `.env` files.
5. Start backend and frontend services.

## Backend

Expected shape:

- Python service under `backend/`
- local configuration supplied through `.env` files

## Frontend

Expected shape:

- frontend application under `frontend/`
- package management through `npm`
- local development server through the frontend scripts

## Environment Variables

Secrets are intentionally not committed.

Use:

- root `.env` for local runtime configuration
- `backend/.env` for backend-specific keys when needed
- `.env.example` as a safe variable-name template

## Rules

- do not commit real API keys
- do not commit machine-specific model paths unless intentionally public
- do not commit dependency folders or generated build output

