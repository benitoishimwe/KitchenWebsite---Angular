# Shop Application · Angular

**Production site**: `https://benitoinhiskitchen.netlify.app`

## Overview

This is a small Angular 13 application for a kitchen / food ordering experience.  
It showcases a simple menu, item details, and static informational pages (home, about, contact).

The project has been structured into:

- **App module**: Application shell and global routing.
- **Pages module**: Feature module for all main pages (home, menu, menu detail, about, contact).
- **Shared module**: Reusable layout elements such as the navbar and footer.

## Getting started

### Prerequisites

- Node.js 16+ (18 recommended)
- npm 8+

### Install and run

```bash
npm install
npm start
```

Then open `http://localhost:4200/` in your browser.

## Available scripts

- **`npm start`**: Run the dev server with live reload.
- **`npm run build`**: Build the application for production.
- **`npm test`**: Run unit tests with Karma/Jasmine.

## CI/CD

GitHub Actions are configured to:

- Run tests and a production build on pushes and pull requests to `master` (`.github/workflows/ci.yml`).
- Perform an automated timestamped commit via the `Auto Commit` workflow.

## Project structure (high level)

```text
src/
  app/
    app.module.ts          # Root module
    app-routing.module.ts  # Root routing, lazy-loads pages
    pages/                 # Feature module and page components
    shared/                # Shared module for layout components
    sharepage/             # Navbar/Footer component implementations
  assets/
  environments/
```

## Contributing

1. Fork the repository and create a feature branch.
2. Run `npm test` and `npm run build` before opening a PR.
3. Open a pull request against `master` with a clear description of your changes.

