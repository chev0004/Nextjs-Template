# Next.js Template by chev

A modern Next.js template with TypeScript, Tailwind CSS v4, and a complete developer experience setup.

## Features

- **Next.js 16** with React 19
- **TypeScript** for type safety
- **Tailwind CSS v4** for styling
- **Biome** for fast linting and formatting
- **React Compiler** enabled for automatic optimizations
- **Git Hooks** (Husky + Commitlint + lint-staged)
  - Pre-commit: Auto-format and lint staged files
  - Commit-msg: Validate conventional commit messages
  - Pre-push: Run full lint and type checks

## Quick Start

```bash
# Install dependencies
bun install

# Start development server
bun dev
```

Visit [http://localhost:3000](http://localhost:3000) to see your app.

## Available Scripts

- `bun dev` - Start development server
- `bun build` - Build for production
- `bun start` - Start production server
- `bun lint` - Run linting checks
- `bun lint:fix` - Fix linting issues automatically
- `bun format` - Format code
- `bun type-check` - Run TypeScript type checking

## Biome Configuration

This template includes a comprehensive Biome setup optimized for Next.js:

**Formatter:**
- 2-space indentation
- 80 character line width
- Single quotes for JavaScript/TypeScript
- Auto-organize imports

**Linter:**
- Next.js domain rules enabled
- Strict rules for unused imports/variables
- Next.js-specific rules (no `<img>`, no `<head>` in pages, etc.)
- Tailwind CSS directive support
- Auto-fix for safe transformations

**Overrides:**
- Allows default exports in Next.js app/pages directories
- Config files and middleware exempt from default export rule

## Commit Convention

This template uses [Conventional Commits](https://www.conventionalcommits.org/). Examples:

- `feat: add user authentication`
- `fix: resolve navigation bug`
- `docs: update README`
- `refactor: simplify component structure`

## Project Structure

```
src/
  └── app/          # Next.js App Router
      ├── layout.tsx
      ├── page.tsx
      └── globals.css
```