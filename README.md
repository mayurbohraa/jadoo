# Jadoo

## Overview

Jadoo is a responsive travel landing page presenting services, destinations, trip-planning steps, and testimonials. Interactive dialogs provide previews of travel and account actions.

## Project Preview

<img src="public/project-preview.webp" alt="Jadoo travel website preview" width="100%">

## Key Features

- Responsive layout with sticky navigation.
- Hotel and flight preview dialogs, destination details, and account dialogs.
- Interactive testimonials, demo popup, trip-save toggle, and newsletter preview.

This is a frontend demonstration. Live search, booking, authentication, and email delivery are not connected. English is the only available language. Footer controls without real URLs show hover feedback but do not navigate.

## Live Website & Related Repository

https://jadoo-lime.vercel.app/

## Tech Stack

- **Interface:** React 19, JavaScript/JSX, Tailwind CSS 4.
- **Tooling:** Vite 7, the React Vite plugin, and Prettier.

## Prerequisites

Node.js 22.12 or newer and npm.

## Installation & Setup

1. Open a terminal in the repository root.
2. Install the locked dependencies.

   ```sh
   npm ci
   ```

3. No environment variables or external service credentials are required for the implemented interface.

## Running Locally

Start development. Vite normally serves http://127.0.0.1:5173/ and prints the actual address if the port is occupied.

```sh
npm run dev
```

Build the static output, then preview it locally.

```sh
npm run build
```

```sh
npm run preview
```

Preview normally serves http://127.0.0.1:4173/. To require the documented development port, use `npm run dev -- --port 5173 --strictPort`.

Check source formatting with the installed formatter:

```sh
npm exec -- prettier --check .
```

Publish `dist/` with a static host. The repository has no automated test, lint, or type-check script.

## Project Structure

```text
public/                 # Public files and README preview
src/
├── assets/             # Images, fonts, icons, logos, and decorations
├── components/
│   ├── layout/         # Header and footer
│   └── ui/             # Shared controls and dialogs
├── data/content.js     # Page content
├── sections/           # Hero, destinations, testimonials, and other sections
├── styles/index.css    # Theme and responsive styles
├── App.jsx             # Page composition
└── main.jsx            # React entry
vite.config.js          # React and Tailwind build integration
```

## Acknowledgements & Credits

- Implemented from the supplied Jadoo UI and visual resources.
- Poppins and Volkhov are bundled with their SIL Open Font License notices in `src/assets/fonts/`.
