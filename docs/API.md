# API

## Response Style

The backend follows a consistent envelope-oriented response style where possible.

Success shape:

```json
{
  "ok": true,
  "message": "optional message",
  "data": {},
  "meta": {}
}
```

Error shape:

```json
{
  "ok": false,
  "error": {
    "code": "machine_readable_code",
    "message": "human readable message"
  },
  "meta": {}
}
```

## Interaction Model

The system is built around chat-style frontend/backend interaction with emphasis on:

- continuity
- response provenance
- stable payload handling
- clear UI-facing behavior

## Public Scope

This file is a high-level overview, not a full internal endpoint reference.

