# Stocks

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()
[![React](https://img.shields.io/badge/React-18-blue)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue)](https://www.typescriptlang.org/)

A React-based Progressive Web App (PWA) for tracking stock price changes over custom date ranges, with support for price change notifications.

## Features

- **Stock Price Tracking:** Enter a ticker and see price changes over a configurable number of business days.
- **Customizable Filters:** Choose price type (open, close, etc.), target date, and notification criteria.
- **Polygon.io Integration:** Fetches real-time and historical price data using your own API key.
- **Notifications:** Get browser notifications when a stock’s price change matches your criteria.
- **PWA Support:** Installable and works offline with persistent state.
- **Modern UI:** Built with React 18, TypeScript, and TanStack Query for robust state and data management.

## Screenshots

> _Add screenshots or demo GIFs here_

![App Screenshot Placeholder](public/favicon.svg)

## Getting Started

### Prerequisites

- Node.js >= 22
- pnpm (recommended, see `package.json`)

### Installation

```bash
pnpm install
```

### Running the App

```bash
pnpm dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Building for Production

```bash
pnpm build
```

### Linting and Formatting

```bash
pnpm lint:check
pnpm format:check
```

## Usage

1. **API Key:** Enter your [Polygon.io](https://polygon.io/) API key.
2. **Ticker:** Enter the stock symbol (e.g., `NVDA`).
3. **Date Range:** Set the number of business days and target date.
4. **Price Type:** Select which price to track (open, close, etc.).
5. **Notifications:** Enable and configure price change alerts.

## PWA Installation

- On desktop or mobile, click the install button in your browser’s address bar or the PWA badge in the app.
- The app works offline and can send notifications if enabled.

## Project Structure

- `src/components/` – UI components (App, SearchForm, SearchResult, etc.)
- `src/functions/` – Data fetching, notification, and utility functions
- `src/fixtures/` – Default values and option definitions
- `src/hooks/` – Custom React hooks
- `public/` – Static assets

## Tech Stack

- React 18 + TypeScript
- Vite (build tool)
- TanStack Query (data fetching/caching)
- Polygon.io client
- PWA support (service workers, offline, installable)
- ESLint & Prettier (code quality)

## Environment Variables

- `VITE_POLY_API_KEY` – (optional) Default Polygon.io API key

## Contributing

Contributions are welcome! Please open issues or pull requests for bug fixes, features, or improvements.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a pull request

## FAQ

**Q: Why do I need a Polygon.io API key?**
A: The app fetches real-time and historical stock data from Polygon.io, which requires an API key.

**Q: Why am I not receiving notifications?**
A: Make sure you have enabled notifications in your browser and granted permission to the app.

**Q: Can I use this app offline?**
A: Yes! The app is a PWA and supports offline usage for previously loaded data.

## License

MIT 
