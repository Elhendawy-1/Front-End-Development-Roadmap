# Front-End-Roadmap

> From Zero to Job-Ready — a step-by-step Arabic-friendly learning path for becoming a front-end developer.

[![Deployed on GitHub Pages](https://img.shields.io/badge/Deployed-GitHub%20Pages-blue)](https://elhendawy-1.github.io/Front-End-Roadmap/)

## Live Demo

**https://elhendawy-1.github.io/Front-End-Roadmap/**

Open the link above to view the roadmap. No build step or server required.

## Overview

This project is a lightweight static website that presents a complete front-end learning roadmap in a single page.

- **What it is:** a curated path with topics, recommended courses, documentation links, hands-on projects, and study guidance.
- **Who it is for:** absolute beginners and self-learners who want a clear order for learning HTML, CSS, JavaScript, TypeScript, React, and related job-ready skills. Course recommendations are primarily in Arabic, with one English alternative for React.
- **Main goal:** take the reader from zero fundamentals to a job-ready front-end developer in an estimated 6–9 months at 2–4 hours of focused study per day.

## Features

Existing functionality in `index.html`:

- Password-gated entry screen (client-side deterrent with 5-attempt limit and 30-second lockout).
- Fixed sidebar navigation with anchor links to each phase and the course summary.
- Dark mode toggle persisted with `localStorage` (with safe fallback when storage is unavailable).
- Phase cards with durations, topic lists, course cards, and project tables.
- Course summary table and official documentation table (MDN, JavaScript.info, React, TypeScript, Git, GitHub).
- Study-method steps, DO / DON'T guidance, and estimated-timeline section.
- Responsive layout — sidebar collapses under 900px (`@media (max-width: 900px)`).
- Security hardening: `rel="noopener noreferrer"` on external links, `referrer`, `X-Content-Type-Options`, and Content-Security-Policy meta tags.
- Inline SVG logo with matching favicon, no external dependencies.

No account system, backend, or automatic progress tracking is implemented — the site is fully static.

## Roadmap Content

Extracted directly from `index.html`:

| # | Stage | Duration | Focus |
|---|-------|----------|-------|
| 0 | Web Fundamentals | 1–2 days | Internet vs Web, client/server, DNS, HTTP/HTTPS, DevTools, VS Code + terminal |
| 1 | HTML + CSS | 4–6 weeks | Semantic HTML, accessibility, CSS fundamentals, Flexbox, Grid, responsive design + 7 projects |
| 2 | JavaScript | 6–10 weeks | Fundamentals, arrays/objects, ES6+, closures/`this`/event loop, DOM, browser APIs, async JS, HTTP/JSON/APIs + 10 projects |
| 3 | Git & GitHub | 1 week | `init`/`add`/`commit`, branches, remotes, repos, PRs, Issues |
| 4 | TypeScript | 2–3 weeks | Types, interfaces, aliases, generics, narrowing, TS with React |
| 5 | React | 4–6 weeks | JSX, components, props/state, hooks, Router, APIs with React |
| 6 | Modern Front-End Skills | 4–6 weeks | Auth, forms/validation, state management, performance, accessibility, deployment, security basics, SEO basics |
| 7 | Testing | 1–2 weeks | Jest, React Testing Library, API mocking, Cypress/Playwright (optional) |
| 8 | Advanced Topics | Ongoing | Junior / intermediate / optional tracks: Next.js, state libraries, WebSockets, GraphQL, CI/CD, micro-frontends, WASM, animation, monorepos |
| ★ | Course Summary | — | Per-phase course table plus official docs links |

Recommended courses referenced in the page: Elzero Web School (HTML, CSS, JavaScript, ES6+, TypeScript), Git & GitHub course, ITI React course, SuperSimpleDev React 19 (English alternative).

## Technologies Used

- HTML5 (single `index.html`, semantic sections and tables)
- CSS3 (custom properties, Flexbox, Grid, media queries — all in inline `<style>`)
- Vanilla JavaScript (DOM handling, `localStorage` — all in inline `<script>`, no frameworks)
- GitHub Pages (static hosting)

## Project Structure

Only files that actually exist in the repository:

```text
Front-End-Roadmap/
├── index.html   # Entire website: markup, styles, and scripts
└── README.md    # This file
```

No build config, package manager, or backend code.

## Getting Started

Clone and run locally (static — just open the file):

```bash
git clone https://github.com/Elhendawy-1/Front-End-Roadmap.git
cd Front-End-Roadmap
```

Then either:

- Double-click `index.html` to open it in your browser, or
- Serve it locally, for example with VS Code Live Server or:

```bash
npx serve .
```

Enter the password configured in `index.html` when prompted by the demo gate.

## Deployment

Hosted with **GitHub Pages** from the `main` branch.

- Push or merge changes to `main`.
- Pages rebuilds automatically, usually live within 1–2 minutes at the Live Demo URL above.
- No build command or environment variables are needed.

## Contributing

Contributions are welcome (content corrections, new resources, UI improvements):

1. Fork the repository.
2. Create a branch: `git checkout -b fix/short-description`.
3. Commit your change: `git commit -m "Describe the fix"`.
4. Push the branch and open a Pull Request against `main`.
5. Describe what changed and why in the PR.

Please keep changes static-friendly (no backend or secrets) and test `index.html` locally before submitting.

## Future Improvements

Planned / potential ideas (not yet implemented):

- Split inline CSS/JS into separate files for stricter CSP and caching.
- Optional progress tracking with `localStorage` (checklist per phase).
- Search/filter across topics and courses.
- Arabic/English language toggle.
- Print-friendly stylesheet and offline (PWA) support.
- Accessibility and Lighthouse performance pass.

## Author

- https://github.com/Elhendawy-1

## License

This repository currently has no specified license (no `LICENSE` file present).
