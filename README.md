# Greenlight

This repository contains the sample API application built while following the "Let's Go Further" book by Alex Edwards (https://lets-go-further.alexedwards.net/). The project is a JSON API for managing a movie catalog, written in Go, and explores many of the techniques used to build production-ready backend services with the Go programming language.

## Features

- JSON API with REST-style endpoints
- Healthcheck endpoint and application metrics
- Browse, create, update, and delete movies
- Filtering, sorting, and pagination for movie listings
- User registration, activation, and authentication
- Permission-based authorization for protected routes
- PostgreSQL database integration with SQL migrations
- Structured logging, panic recovery, and rate limiting middleware
- Background email sending for user activation workflows
- Makefile tasks for development, auditing, building, and deployment
- Production deployment assets for `systemd` and Caddy

## Project Layout

The code is organized using conventions described in the book:

```text
cmd/api/              # entry point and HTTP handlers for the JSON API
cmd/examples/         # small example programs from the book
internal/data/        # data models, queries, and database-related types
internal/jsonlog/     # structured JSON logging helpers
internal/mailer/      # email sending logic and templates
internal/validator/   # reusable validation helpers
internal/vcs/         # build/version metadata helpers
migrations/           # SQL migration files
remote/production/    # production service and Caddy config
remote/setup/         # server bootstrap scripts
```
