# Security

## Core Rules

- keep the working source repository private unless content is intentionally curated for release
- never commit `.env` files with real secrets
- never commit private SSH keys
- never commit local memory or user-derived data

## Release Hygiene

For public sharing:

- prefer a separate public repository
- publish only reviewed documentation
- avoid internal roadmaps and audits
- avoid machine-local paths and development-only notes

## Private-First Philosophy

FPGA-Mind is built with the assumption that useful AI systems often need private context, local state, and careful secret handling.

That is why the public surface should stay intentionally smaller than the internal project surface.

