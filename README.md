from pathlib import Path

content = """# Next.js Dashboard

A full-stack dashboard application built with **Next.js**, **React**, **TypeScript**, and **Tailwind CSS**. This project is intended to explore the core features of modern Next.js development, from page routing and styling to database integration, authentication, and deployment.

## Features

- **Styling:** Build responsive pages and reusable UI components with Tailwind CSS.
- **Routing and layouts:** Use the Next.js App Router to create pages, nested layouts, and dashboard routes.
- **Optimizations:** Optimize images, links, fonts, and page performance with Next.js features.
- **Data fetching:** Fetch and display dynamic data, with support for PostgreSQL when configured.
- **Search and pagination:** Use URL search parameters to filter and paginate dashboard data.
- **Data mutations:** Create, update, and delete records with Server Actions and revalidate cached data.
- **Error handling:** Handle application errors and missing pages with error and not-found UI.
- **Forms and accessibility:** Add server-side validation and accessible form controls.
- **Authentication:** Add authentication and protect private dashboard routes when configured.
- **Metadata:** Configure page titles, descriptions, and social-sharing metadata.

> Features will be implemented progressively as the project develops.

## Tech Stack

- [Next.js](https://nextjs.org/docs)
- [React](https://react.dev/)
- [TypeScript](https://www.typescriptlang.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [pnpm](https://pnpm.io/)
- PostgreSQL and an authentication solution may be added as needed.
- [Vercel](https://vercel.com/) for deployment (optional).

## Project Structure

```text
nextjs-dashboard/
├── app/                    # Application routes, pages, and layouts
├── public/                 # Static assets
├── .gitignore              # Files excluded from Git
├── README.md               # Project documentation
├── next-env.d.ts           # Next.js TypeScript declarations
├── next.config.ts          # Next.js configuration
├── package.json            # Scripts and dependencies
├── pnpm-lock.yaml          # Locked dependency versions
├── pnpm-workspace.yaml     # pnpm workspace configuration
├── postcss.config.js       # PostCSS configuration
├── tailwind.config.ts      # Tailwind CSS configuration
└── tsconfig.json           # TypeScript configuration
```

The exact files and configuration may vary by Next.js and Tailwind CSS version.

## Getting Started

### Prerequisites

- Node.js version supported by your installed Next.js version
- pnpm

### Install dependencies

From the project root, run:

```bash
pnpm install
```

### Start the development server

```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Available scripts

Check the `scripts` section of `package.json` for the exact commands available in this project. A typical Next.js project includes:

```bash
pnpm dev       # Start the development server
pnpm build     # Build for production
pnpm start     # Start the production server
pnpm lint      # Run linting, if configured
```

Only run scripts that are present in your `package.json`.

## Environment Variables

If you add a database or authentication provider, create a local `.env.local` file and define the required variables there. Keep secrets out of version control.

You can document required variable names in a committed `.env.example` file using empty or placeholder values. Never put real credentials in `.env.example` or commit them to Git.

## Development Roadmap

- [ ] Build the dashboard layout and navigation.
- [ ] Create responsive pages and reusable components.
- [ ] Add data fetching and database integration.
- [ ] Implement search and pagination.
- [ ] Add create, update, and delete operations.
- [ ] Add form validation and accessible error messages.
- [ ] Configure authentication and protected routes.
- [ ] Add metadata and social-sharing previews.
- [ ] Test the production build and deploy the application.

## Deployment

The application can be deployed to [Vercel](https://vercel.com/) or another platform that supports Next.js.

Before deploying, verify the production build, configure any required environment variables, and connect any external services the application uses.

## Learning Resources

- [Next.js Documentation](https://nextjs.org/docs)
- [Next.js Learn](https://nextjs.org/learn)
- [React Documentation](https://react.dev/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [pnpm Documentation](https://pnpm.io/motivation)

## License

No license has been specified yet. Add a license if you plan to distribute or reuse this project publicly.
"""

path = Path("/mnt/data/README.md")
path.write_text(content, encoding="utf-8")
print(f"Created {path}")
