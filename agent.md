# Agent Development Guide

This document is designed to help AI agents understand the project context, structure, and guidelines for rapid iteration and development.

## 1. Project Overview
- **Name**: web
- **Type**: Single Page Application (SPA)
- **Framework**: React + TypeScript
- **Build Tool**: Vite

## 2. Tech Stack
- **Core**: React 18+, TypeScript
- **Styling**: CSS Modules / Standard CSS (Current: `App.css`, `index.css`)
- **Linting**: ESLint
- **Package Manager**: npm

## 3. Project Structure
```
/web
├── public/              # Static assets (favicons, manifest, etc.)
├── src/                 # Source code
│   ├── assets/          # Images, fonts, etc.
│   ├── components/      # Reusable UI components (Create this folder if needed)
│   ├── App.tsx          # Main application component
│   ├── main.tsx         # Entry point
│   └── index.css        # Global styles
├── index.html           # HTML template
├── package.json         # Dependencies and scripts
└── vite.config.ts       # Vite configuration
```

## 4. Development Workflow

### Commands
- **Start Dev Server**: `npm run dev` (Runs on http://localhost:5173 or next available port)
- **Build for Production**: `npm run build`
- **Preview Build**: `npm run preview`
- **Lint**: `npm run lint`

### Convention Guidelines
- **Component Structure**: Functional components with Hooks.
- **Naming**: PascalCase for components (e.g., `MyComponent.tsx`), camelCase for functions/variables.
- **State Management**: Use `useState`, `useReducer`, or Context API for local state.
- **Styling**: Prefer CSS modules or utility classes for component-level styling to avoid conflicts.

## 5. Task Tracking
*Use this section to track current and future tasks.*

- [ ] [Feature] Add initial component structure
- [ ] [UI] Improve basic styling
- [ ] [Docs] Update README.md with specific project details

## 6. Notes for Agent
- Always check `package.json` for the latest dependencies.
- When adding new features, ensure to update this document if architectural changes occur.
- Prefer small, incremental changes verified by running the dev server.
