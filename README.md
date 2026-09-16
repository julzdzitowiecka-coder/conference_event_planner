# Conference Expense Planner

React + Redux app for planning conference budgets.

The user selects venue rooms, AV equipment, and meal options — the app calculates a live cost breakdown per category and shows a final itemised summary. Meal costs scale automatically based on the number of attendees.

## Tech Stack

- React 18, Redux Toolkit
- Slices: `venueSlice`, `avSlice`, `mealsSlice`

## Project Structure

```
src/
├── ConferenceEvent.jsx   # Main component
├── TotalCost.jsx         # Summary view
├── venueSlice.js
├── avSlice.js
└── mealsSlice.js
```

## Getting Started

```bash
npm install
npm start
```

## Usage

1. **Venue** — `+` / `−` to select rooms (max quantity per type enforced)
2. **Add-ons** — `+` / `−` to add AV equipment
3. **Meals** — enter number of attendees, check desired meal options
4. **Show Details** — view full itemised cost breakdown

## Known Issues

- `numberOfPeople` resets on page refresh (not persisted)
- `class` instead of `className` on `.meal_item` div — React console warning
