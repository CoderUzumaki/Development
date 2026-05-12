# Development

## Next.js

Next.js is a React framework for building full-stack web applications. It provides features like server-side rendering, static site generation, and API routes.

## Next.js Project Specifications

### Application Structure

A typical Next.js application should keep route files, UI components, and shared utilities clearly separated:

```text
.
├── app/
│   ├── layout.tsx
│   ├── page.tsx
│   └── api/
├── components/
├── lib/
├── public/
└── next.config.js
```

### Core Requirements

- Use the App Router for new pages and layouts.
- Keep reusable interface elements in `components/`.
- Store framework-agnostic helpers in `lib/`.
- Place static assets such as images and icons in `public/`.
- Use API routes only for server-side work that should not run in the browser.

### Rendering Options

Next.js supports several rendering patterns:

- Server Components for data-heavy UI that can render on the server.
- Client Components for interactive UI that needs browser state or events.
- Static generation for pages that rarely change.
- Dynamic rendering for pages that depend on request-time data.

### Recommended Development Flow

1. Create or update routes in the `app/` directory.
2. Build reusable UI in `components/`.
3. Add data fetching and validation in server-side utilities.
4. Test the page locally with `npm run dev`.
5. Run a production build before deployment.

### Deployment Notes

Next.js applications are commonly deployed to Vercel, but they can also run on any Node.js hosting provider that supports the selected rendering mode. Always check environment variables, build output, and server-only secrets before deployment.
