# NoteHub

![Next.js](https://img.shields.io/badge/next.js-000000.svg?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/react-20232A.svg?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/typescript-3178C6.svg?style=for-the-badge&logo=typescript&logoColor=white)
![TanStack Query](https://img.shields.io/badge/tanstack%20query-FF4154.svg?style=for-the-badge&logo=reactquery&logoColor=white)

> NoteHub is a note management web application for creating, browsing, filtering,
> previewing, and organizing personal notes in a clean authenticated workspace.

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation and Running](#installation-and-running)

## About the Project

NoteHub is built as a modern full-stack frontend application with protected
routes, server-rendered pages, and client-side interactivity. It provides a
simple workflow for managing personal notes while keeping the interface fast and
focused.

The application allows users to:

- register and sign in;
- browse notes by tag;
- search notes by keyword;
- paginate through note collections;
- open note previews in a modal;
- open full note detail pages;
- create new notes;
- delete existing notes;
- view and edit profile information.

## Features

- Authentication flow with sign-in, sign-up, logout, and protected routes.
- Notes dashboard with search, tag-based filtering, and pagination.
- Dedicated note detail pages with direct routing.
- Intercepted modal route for note preview without leaving the list view.
- Create note form with persistent draft state.
- Profile page with editable user information.
- Server-side and client-side data fetching depending on the route.
- Responsive UI built with CSS Modules and a shared global design system.

## Tech Stack

- Core:
  - Next.js 16
  - React 19
  - TypeScript
- Data and state:
  - TanStack React Query
  - Zustand
- Forms and validation:
  - Formik
  - Yup
- Networking and utilities:
  - Axios
  - cookie
  - use-debounce
  - react-paginate
- Styling and tooling:
  - CSS Modules
  - ESLint
  - modern-normalize

## Project Structure

- `app/` — App Router pages, layouts, API routes, modal routes, and metadata
- `components/` — reusable UI components such as header, footer, note list,
  pagination, search box, modal, and forms
- `lib/api/` — client and server API helpers
- `lib/store/` — Zustand stores for auth and note draft state
- `types/` — shared TypeScript types for notes and users

## Installation and Running

### Prerequisites

- Node.js 18 or newer
- npm

### Environment Variables

Create an `.env.local` file and define the API base URL:

```env
NEXT_PUBLIC_API_URL=your_api_base_url
```

### Steps

1. Clone the repository.
2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm run dev
```

4. Open the app in the browser:

```text
http://localhost:3000
```

### Available Scripts

```bash
npm run dev
npm run build
npm run start
npm run lint
```
