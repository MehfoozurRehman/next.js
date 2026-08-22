# Next.js: The React Framework for the Web

Next.js is the flexible React framework that gives building blocks to create fast, full-stack web applications.

## Overview

This repository houses the core source code, compilers, Turbopack integration, SWC bindings, and monorepo packages for Next.js:
- **`packages/next`**: Core runtime, CLI, server handlers, and build tooling.
- **`packages/next-swc`**: Rust-based compilation and minification engine.
- **`packages/create-next-app`**: Interactive CLI for scaffolding Next.js applications.
- **`examples/`**: Curated library of framework recipes, integrations, and starter templates.

## Tech Stack

- **Core Engine**: Rust (SWC / Turbopack), TypeScript, React (React Server Components)
- **Monorepo Tooling**: [Turborepo](https://turbo.build/), pnpm workspaces, Lerna
- **Testing**: Jest, Playwright, Edge Runtime, Replay.io

## Prerequisites

- Node.js (v18.17+ or v20+)
- Package manager (`pnpm` v8+ recommended)
- Rust toolchain (for building native SWC packages)

## Getting Started

1. **Install workspace dependencies**:
   ```bash
   pnpm install
   ```

2. **Build Packages with Turborepo**:
   ```bash
   pnpm prepublishOnly
   # or
   pnpm turbo run build
   ```

3. **Run Framework Tests**:
   ```bash
   pnpm test
   ```

## Available Scripts

- `pnpm turbo run build` - Builds all packages across the workspace.
- `pnpm test` - Runs the comprehensive Next.js integration test suite.
- `pnpm lint` - Performs ESLint and type checks.
- `pnpm prettier-fix` - Formats the codebase.

## Author

Created by [Mehfooz-ur-Rehman](https://github.com/MehfoozurRehman).
