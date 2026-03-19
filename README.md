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

The application allows users to create and manage personal notes in one place, with authentication, tag-based
organization, keyword search, pagination, quick modal previews, full note
detail pages, and basic profile management.

## Features

NoteHub combines protected user flows with a practical note-management
interface. Authenticated users can browse notes in a paginated dashboard,
filter them by tag, search by keyword, open quick previews in a modal, navigate
to dedicated note pages, create new notes, remove old ones, and update profile
information. The application also mixes server-rendered and client-rendered
data fetching to keep navigation responsive while preserving direct-route
support.

## Tech Stack

- Core:
  - [Next.js 16](https://nextjs.org/)
  - [React 19](https://react.dev/)
  - [TypeScript](https://www.typescriptlang.org/)
- Data and state:
  - [TanStack React Query](https://tanstack.com/query/latest)
  - [Zustand](https://zustand-demo.pmnd.rs/)
- Forms and validation:
  - [Formik](https://formik.org/)
  - [Yup](https://github.com/jquense/yup)
- Networking and utilities:
  - [Axios](https://axios-http.com/)
  - [cookie](https://www.npmjs.com/package/cookie)
  - [use-debounce](https://github.com/xnimorz/use-debounce)
  - [react-paginate](https://github.com/AdeleD/react-paginate)
- Styling and tooling:
  - [CSS Modules](https://github.com/css-modules/css-modules)
  - [ESLint](https://eslint.org/)
  - [modern-normalize](https://github.com/sindresorhus/modern-normalize)

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
