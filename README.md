Here's a README you can use — based entirely on what I read in the codebase:

````markdown
# Pronto Pizza 🍕

A fast, minimal pizza ordering web app built with React. Browse the menu, build your cart, and place orders — no account needed.

## Features

- Browse a live pizza menu fetched from a remote API
- Add, remove, and update item quantities in the cart
- Place orders with a name, phone number, and delivery address
- Auto-detect your current location for the address field
- Mark an order as priority (+20% price) before or after placing it
- Look up any existing order by its ID
- Fully responsive layout

## Tech Stack

| Tool            | Purpose                                |
| --------------- | -------------------------------------- |
| React 18        | UI                                     |
| React Router v6 | Client-side routing, loaders & actions |
| Redux Toolkit   | Global state (cart, user)              |
| Tailwind CSS    | Styling                                |
| Vite            | Build tool                             |

## Getting Started

```bash
npm install
npm run dev
```
````

Open [http://localhost:5173](http://localhost:5173) in your browser.

## Scripts

| Command           | Description                      |
| ----------------- | -------------------------------- |
| `npm run dev`     | Start development server         |
| `npm run build`   | Production build                 |
| `npm run preview` | Preview production build locally |
| `npm run lint`    | Run ESLint                       |

## Project Structure

```
src/
├── features/
│   ├── cart/        # Cart state (Redux slice) and cart UI
│   ├── menu/        # Menu fetching and display
│   ├── order/       # Order creation, tracking, and update
│   └── user/        # Username and geolocation address
├── services/
│   ├── apiRestaurant.js   # Menu and order API calls
│   └── apiGeocoding.js    # Reverse geocoding (BigDataCloud)
├── ui/              # Shared layout components
└── utils/           # Currency and date helpers
```

## API

This app uses the [Jonas Schmedtmann Pizza API](https://react-fast-pizza-api.jonas.io/api) for menu and order data, and [BigDataCloud](https://www.bigdatacloud.com/) for reverse geocoding.

```

```
