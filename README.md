# TapaPalavras Frontend

A modern web application for the TapaPalavras word game built with Next.js 15, React 19, and Socket.IO for real-time multiplayer functionality.

## Features

- Real-time multiplayer word game
- Responsive design using Tailwind CSS
- Modern React with server and client components
- Socket.IO integration for real-time updates

## Tech Stack

- **Framework**: Next.js 15
- **UI Library**: React 19
- **Styling**: Tailwind CSS
- **Real-time Communication**: Socket.IO
- **Language**: TypeScript

## Getting Started

### Prerequisites

- Node.js 18+
- Yarn or npm

### Installation

1. Clone this repository
2. Install dependencies:

```bash
yarn install
# or
npm install
```

3. Create a `.env` file in the root directory with:

```
NEXT_PUBLIC_API_URL=http://localhost:3001
```

### Development

Run the development server:

```bash
yarn dev
# or
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Building for Production

```bash
yarn build
# or
npm run build
```

Then start the production server:

```bash
yarn start
# or
npm start
```

## Project Structure

- `/src/app`: Next.js app router pages and layouts
- `/src/components`: Reusable UI components
- `/src/contexts`: React contexts for state management
- `/src/lib`: Utility functions and shared code
- `/src/types`: TypeScript type definitions

## Connecting to the API

The frontend connects to the TapaPalavras API via Socket.IO for real-time game functionality. Make sure the API is running (see the API README) and the `NEXT_PUBLIC_API_URL` environment variable points to the correct API endpoint.
