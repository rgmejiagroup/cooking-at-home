# Cooking-at-Home API – Overview

Welcome to the Cooking-at-Home API! This API enables users to organize, share, and explore recipes via a cloud-based cookbook system.

## What does this API do?

The Cooking-at-Home API offers endpoints to:
- Add, view, and delete recipes
- Manage user profiles
- Share recipes across user accounts
- Organize and access shared meal planning data

## Who is this API for?

This API is designed for:
- Home cooks and professionals sharing recipes
- Cooking educators and students
- Families organizing weekly meal plans
- Anyone seeking a collaborative, cloud-based kitchen companion

## How does it work?

The API is REST-based and supports standard JSON-formatted requests. Most actions involve sending POST, GET, PATCH, or DELETE calls to the `/recipes` and `/users` endpoints.

## Prerequisites

Before using the API, developers should:
- Have basic knowledge of RESTful APIs
- Set up authentication via token header (to be added in future version)
- Register a user account through the `/users` resource

## Suggested Topics and Structure

### Essential Topics
- `GET /recipes`
- `GET /users`
- `POST /recipes`
- `PATCH /recipes/{id}`
- `DELETE /recipes/{id}`

### Optional Topics
- `GET /shared-recipes`
- `PATCH /users/preferences`
- `POST /feedback`

## Where to Go Next

You can explore:
- [API References](../api/)
- [Tutorials](../tutorials/)
- [Quick Start Guide](../index.md)
