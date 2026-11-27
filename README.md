# PulseWorks AI

A beginner-friendly task dashboard made with React, Vite, and Zod.

## Get started

1. Copy `.env.example` to `.env`.
2. Run `npm install`.
3. Run `npm run dev`.

The task form checks new tasks in your browser using the strict schema in
`src/schemas/taskSchema.js`. Tasks are kept in page state and are not saved to a
server yet.

## Workspace pages

- **Tasks**: create, search, filter, complete, and persist tasks in local storage.
- **Analytics**: view task progress and safely loaded activity from a public external API.
- **Settings**: update workspace preferences saved in local storage.

Set `VITE_API_BASE_URL` to an HTTPS API root in `.env`. The app validates JSON
responses with Zod, aborts slow or unmounted requests, and shows loading and
error states without exposing API credentials.
