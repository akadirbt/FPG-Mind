# Architecture

## High-Level Shape

FPGA-Mind is organized around two major layers:

- `backend/` for orchestration, API handling, memory, search, and response flow
- `frontend/` for the user-facing web experience

## Backend Responsibilities

The backend handles:

- request processing
- conversation flow
- memory and continuity logic
- search and grounding workflows
- response shaping for the UI

## Frontend Responsibilities

The frontend handles:

- chat interaction
- session rendering
- user controls
- message display and flow

## System Direction

The project is designed to feel personal without becoming sloppy.

That means:

- memory is treated carefully
- grounding matters more than stylistic confidence
- local state should stay under control
- modular structure matters as the system grows

## Public Boundary

This public documentation intentionally avoids exposing:

- internal roadmap material
- implementation-level control-plane details
- local file and environment structure that should stay private
- internal audit and debugging workflows

