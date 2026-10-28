# Daily Task Tracker

A gamified mobile app that gives you a fresh set of daily tasks every day. Complete them before the midnight countdown runs out, climb the leaderboard, and spend what you earn in the shop.

Built as a team project for **CSC 131 (Software Engineering)** at Sacramento State, Spring 2026.

## Features

- **Daily tasks** that reset every night at midnight, with an option to reroll a task
- **Countdown timer** showing how long is left until the next set of tasks
- **Accounts**: sign up, log in, and reset a forgotten password (Supabase Auth)
- **Leaderboard**, **Profile**, and **Shop** tabs

## Tech stack

| Layer | Tools |
| --- | --- |
| App | React Native 0.81, Expo SDK 54, Expo Router |
| Language | TypeScript |
| Backend | Supabase (auth + database) |
| UI | React Native Elements, Expo vector icons |

## My contribution

I built the **user interface** and the **countdown timer** (`src/components/CountdownTimer.tsx`). The timer counts down to local midnight, displays it as `HH:MM:SS`, and triggers the daily task reset when it hits zero.

## Team

- Collins Nyamu
- Luke
- Hiroshi Karunaratne

Original repository: [CollinsNyamu/CSC131](https://github.com/CollinsNyamu/CSC131)

## Run it locally

```bash
npm install
npx expo start
```

Then open it in Expo Go on your phone, or press `w` to run it in the browser. You'll need a Supabase project URL and key in `src/.env`:

```
EXPO_PUBLIC_SUPABASE_URL=your-project-url
EXPO_PUBLIC_SUPABASE_KEY=your-publishable-key
```
