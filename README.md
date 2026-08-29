<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/branding/icon.svg" />
  <source media="(prefers-color-scheme: light)" srcset="assets/branding/icon-dark.svg" />
  <img src="assets/branding/icon-dark.svg" alt="Halterofit icon" width="130" />
</picture>

<img src=".github/social-preview.png" alt="Halterofit app showcase" width="100%" />

</div>

<br/>

## About

Halterofit is a workout-tracking app for lifters who take their training seriously: browse 1,500+
exercises, build your own multi-day plans, log every set at the gym and watch your strength
move over time. Everything works without a connection — the app keeps its data on the phone and
syncs to the cloud when it can.

Built solo, from scratch, as a production mobile app rather than a tutorial project. This repository
is its public face; the code stays private.

## What it does

- **Exercise library** — 1,500+ exercises with animated demonstrations, and an interactive body map:
  tap a muscle to see the exercises that target it.
- **Plan builder** — multi-day programs you arrange by drag-and-drop, days and exercises alike.
- **Set logging** — built for the gym floor: a few taps per set, a rest timer between them.
- **Progress** — estimated one-rep max, volume and personal records, computed on the device.
- **Insights** — coaching findings computed from your own history — plateaus, readiness to progress,
  volume balance across muscles — each one showing the sets it comes from.
- **Offline-first** — every feature works with no signal; sync happens in the background when a
  connection returns.

## How it's built

| Layer        | Technology                                                                         |
| ------------ | ---------------------------------------------------------------------------------- |
| **App**      | React Native + Expo (New Architecture, React Compiler), TypeScript strict, Expo Router |
| **Data**     | WatermelonDB (SQLite) on the device, bidirectional sync to Supabase (Postgres + Auth) |
| **State**    | Zustand, MMKV                                                                      |
| **UI**       | NativeWind, Reanimated, Skia charts, FlashList                                     |
| **Delivery** | pnpm + Turborepo monorepo, EAS Build, Sentry                                       |

## Engineering highlights

- A real offline-first architecture: a full local database with bidirectional sync and soft deletes,
  not cached API calls.
- Analytics and coaching insights computed deterministically on the device — the same data always
  gives the same answer, and every number traces back to logged sets.
- Custom drag-to-reorder running on the UI thread with Reanimated gesture handlers.
- An interactive SVG body map with per-muscle tap detection.

## About this repository

> This is a **showcase repository**: the source code is maintained in a private repository.
>
> <sub>Maintainer note — nothing syncs this page with the app, so it states only what does not change: no versions, no counts, no phase status. A line that needs a number to stay true does not belong here.</sub>

I built Halterofit to learn production mobile development by shipping one, and it is still in active
development. For a code walkthrough, a live demo, or the reasoning behind the technical decisions,
reach out.

**Patrick Patenaude**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/patrickpatenaude/)
[![Email](https://img.shields.io/badge/Email-contact@halterofit.ca-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:contact@halterofit.ca)
[![Portfolio](https://img.shields.io/badge/Portfolio-halterofit.ca-0EA5E9?style=for-the-badge&logo=safari&logoColor=white)](https://halterofit.ca)
