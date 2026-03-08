# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

- **Dev server**: `npm run dev` (starts on localhost:3000)
- **Build**: `npm run build`
- **Start production**: `npm run start`
- **Lint**: `npm run lint` (ESLint with Next.js core-web-vitals and TypeScript rules)

## Architecture

- **Framework**: Next.js 16 with App Router, React 19, TypeScript (strict mode)
- **Styling**: Tailwind CSS v4 via `@tailwindcss/postcss` plugin; theme uses CSS custom properties for light/dark mode (`prefers-color-scheme`)
- **Fonts**: Geist sans and mono via `next/font/google`, applied as CSS variables
- **Path alias**: `@/*` maps to `./src/*`

## Project Structure

All application code lives under `src/app/` using the Next.js App Router convention:
- `layout.tsx` — root layout with font setup and metadata
- `page.tsx` — route page components
- `globals.css` — Tailwind import and theme CSS variables
