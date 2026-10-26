# Campus Event Hub

A futuristic, responsive campus-events frontend built with React, Vite, Tailwind CSS v4, Framer Motion, and Lucide React. This is a browser-only prototype; it does not use a backend or send email.

## Requirements
- Node.js 20.19+ (or a compatible current LTS release)
- npm
- VS Code (recommended)

## Run locally
Open this folder in VS Code, open Terminal → New Terminal, and run:

```bash
npm install
npm run dev
```

Open the local URL printed by Vite (normally `http://localhost:5173`).

## Production build

```bash
npm run build
npm run preview
```

## Included features
- Futuristic dark UI with optional light theme; theme preference persists in LocalStorage.
- Responsive layout and mobile navigation.
- Sample event cards with date, venue, organizer, category, seat capacity, and registration deadline.
- Live search, category filters, availability filter, date sorting, reset filters, and saved-only view.
- Event details modal with Escape and outside-click close behavior.
- Registration form with required-field, email, optional phone, duplicate-registration, capacity, and deadline checks.
- Confirmation screen and registration ID.
- My Registrations dashboard with upcoming count and cancel confirmation.
- Bookmark/save events and LocalStorage persistence.
- Motion effects, responsive layout, visible keyboard focus, and reduced-motion support.

## Frontend-only limitations
- All event records and registrations are demo data stored in the current browser's LocalStorage. They are not shared across students, browsers, or devices.
- LocalStorage is not secure storage. Do not enter sensitive or real student information into a public demo.
- Registration confirmation is local only. No email is sent and no server confirms seats.
- Event capacity updates only in the current browser. A production deployment needs a backend, database, authentication, and server-side validation.

## Project structure

```text
campus-event-hub/
├── index.html
├── package.json
├── vite.config.js
├── README.md
└── src/
    ├── App.jsx
    ├── index.css
    ├── main.jsx
    └── data/
        └── events.js
```
