# FitLog

FitLog is a workout planner for browsing exercises and organizing a daily routine. Review exercise details, add exercises to today's plan or save them for later, and track estimated workout time and calories.

## Features

- Browse an exercise library with descriptions, instructions, equipment, difficulty, sets, reps, duration, calories, and ratings.
- Add exercises to today's plan or save them for later.
- View exercise and calorie totals, and total duration for the selected list.
- Sort planned and saved exercises by duration, calories, or rating.
- Remove exercises from either list.
- Get toast notifications for list actions.

## Getting Started

### Requirements

- Node.js
- npm

### Install and run

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Available Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the local development server. |
| `npm run build` | Create a production build. |
| `npm start` | Run the production server after building. |
| `npm run lint` | Run ESLint. |

## Using FitLog

1. Browse the exercise library on the home page.
2. Open an exercise to read its details and instructions.
3. Add it to today's plan or save it for later.
4. Open **My Plan** to switch between today's plan and saved exercises, review totals, sort the list, or remove an exercise.

Plan and saved-list data is kept in React context while the app is running; it is not persisted across page reloads.

## Data Source

The exercise library and detail pages request data from `https://api.abcz.workers.dev/api/fitlog`. The app currently has no local exercise database.

## Tech Stack

- Next.js and React
- JavaScript and JSX
- Tailwind CSS and DaisyUI
- React Toastify

## Project Structure

```text
src/
	app/          App Router pages and global styles
	components/   Exercise, plan, navigation, and footer components
	Contexts/     Shared exercise-plan state
```
