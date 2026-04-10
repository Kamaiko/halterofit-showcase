<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/branding/icon.svg" />
  <source media="(prefers-color-scheme: light)" srcset="assets/branding/icon-dark.svg" />
  <img src="assets/branding/icon-dark.svg" alt="Halterofit icon" width="130" />
</picture>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/branding/wordmark.png" />
  <source media="(prefers-color-scheme: light)" srcset="assets/branding/wordmark-dark.png" />
  <img src="assets/branding/wordmark-dark.png" alt="Halterofit" width="360" />
</picture>

<img src=".github/social-preview.png" alt="Halterofit app showcase" width="100%" />

<br/>

🇫🇷 <a href="README-fr.md">Lire en français</a>

</div>

<br/>

## About

A fitness tracking app built for lifters who take their training seriously. Browse 1,300+ exercises with animated GIF demonstrations, build custom workout plans with drag-to-reorder, and discover pre-built training programs — all offline-first. Built entirely solo from scratch.

<div align="center">
<img src="assets/diagrams/user-lifecycle.svg" alt="User Lifecycle — from discovery to progress" width="100%" />
</div>

<br/>

## Features

<div align="center">
<img src="assets/diagrams/appfeature.png" alt="Why Athletes Trust This App" width="100%" />
</div>

### Exercise Library
Browse **1,300+ exercises** from the ExerciseDB database. Each exercise includes animated GIF demonstrations, step-by-step instructions, and an **interactive muscle highlighter** — tap any muscle on a full-body diagram to see which exercises target it.

### Workout Planning
Build **custom multi-day plans** with full drag-to-reorder support for both days and exercises. Edit day names, add exercises from the library, and organize your training week exactly how you want.

### Plans Marketplace
Browse and acquire **pre-built training programs** — filter by category (Strength, Hypertrophy, Beginner, Powerlifting) and pricing (Free / Premium). Acquired plans are fully editable.

### Offline-First
**Every feature works without internet.** All data is stored on-device via WatermelonDB (SQLite) and syncs to Supabase PostgreSQL when a connection is available. Zero data loss, even mid-workout.

### Dark Mode First
Designed for **gym environments** — high contrast dark UI that's easy to read between sets, even in dim lighting.

<br/>

## Tech Stack

| Category | Technology |
|----------|-----------|
| **Framework** | React Native 0.81 · Expo SDK 54 · New Architecture (Fabric) |
| **Language** | TypeScript (strict mode) |
| **Navigation** | Expo Router v3 (file-based routing) |
| **Database** | WatermelonDB (offline-first SQLite) |
| **Backend** | Supabase (Auth + PostgreSQL + sync) |
| **State** | Zustand + react-native-mmkv |
| **Styling** | NativeWind v4 + Tailwind CSS |
| **Animations** | React Native Reanimated 4 |
| **Lists** | FlashList 2.0 |
| **Build** | pnpm + Turborepo monorepo · EAS Build |
| **Monitoring** | Sentry |
| **Optimization** | React Compiler (automatic memoization) |

<br/>

## Architecture

- **Monorepo** — pnpm workspaces + Turborepo (mobile app, planned web companion, shared packages)
- **Offline-first sync** — WatermelonDB on device ↔ bidirectional sync ↔ Supabase PostgreSQL
- **Layered architecture** — Screens → Components → Hooks → Services → Stores

<br/>

## Project Highlights

- Built **entirely solo** from zero to production-ready
- **New Architecture** (Fabric renderer) enabled from day one
- **React Compiler** for automatic performance optimization
- Real **offline-first** — full local database with bidirectional sync, not cached API calls
- Custom **drag-to-reorder** built with Reanimated gesture handlers on the UI thread
- **Interactive SVG body diagram** with per-muscle tap detection

<br/>

## About This Repository

> This is a **showcase repository**. The source code is maintained in a private repository.

I built Halterofit as a solo project to push my skills in React Native and production mobile development. This is an ongoing project — I'm actively building new features and refining the UX.

For a code walkthrough, live demo, or to discuss the technical decisions behind this project, feel free to reach out.

**Patrick Patenaude**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/patrickpatenaude/)
[![Email](https://img.shields.io/badge/Email-contact@halterofit.ca-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:contact@halterofit.ca)
[![Portfolio](https://img.shields.io/badge/Portfolio-halterofit.ca-0EA5E9?style=for-the-badge&logo=safari&logoColor=white)](https://halterofit.ca)
