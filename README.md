# TapaPalavras 🎮

A real-time multiplayer word game inspired by the classic group word-association games. Players take turns selecting letters and creating words based on a theme, racing against the clock!

![TapaPalavras Game](https://via.placeholder.com/800x400?text=TapaPalavras+Game)

## 🎯 How to Play

1. **Create a Room**: Start by creating a new game room and share the room code with your friends.
2. **Set a Theme**: As the host, enter a custom theme for the round (e.g., Animals, Countries, Movies).
3. **Take Turns**: Players take turns selecting a letter from the wheel and saying a word related to the theme that contains that letter.
4. **Beat the Clock**: You have 10 seconds to select a letter and come up with a word!
5. **Win Together**: Work together to use all letters on the board before time runs out.

## 🌟 Features

- **Real-time Multiplayer**: Play with friends from anywhere with WebSocket-based real-time gameplay.
- **Custom Themes**: The host can set any theme they want for each round.
- **Visual Letter Wheel**: Interactive circular letter selector inspired by the physical game.
- **Turn Timer**: Adds excitement with a countdown timer for each player's turn.
- **Responsive Design**: Play on desktop or mobile devices with a fully responsive interface.
- **Debug Mode**: Add `?debug=true` to the URL to see detailed game state information.

## 🛠️ Technical Stack

- **Frontend**: Next.js, React, TypeScript, Tailwind CSS
- **Backend**: Node.js, Express, Socket.IO
- **State Management**: React Context API
- **Styling**: Tailwind CSS with custom color palette

## 🚀 Getting Started

### Prerequisites

- Node.js (v14+ recommended)
- npm or yarn

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/pedrobarretto/tapalavras.git
   cd tapalavras
   ```

2. Install dependencies for both client and server:

   ```bash
   # Install client dependencies
   npm install

   # Install server dependencies
   cd server
   npm install
   ```

3. Start the development servers:

   ```bash
   # Start the server (from the server directory)
   npm run dev

   # In a new terminal, start the client (from the root directory)
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:3000`

## 🎮 Gameplay Rules

- A theme is selected by the host at the beginning of each round
- Letters are randomly arranged in a circle
- Each player has 10 seconds to:
  - Select an unused letter
  - Say a word related to the theme containing that letter
  - Pass the turn to the next player
- If a player fails to complete their turn in time, the game ends
- The game is won when all letters have been successfully used

## 🧩 Project Structure

```
├── public/            # Static assets
├── server/            # Backend server code
│   ├── src/           # Server source code
│   │   └── index.ts   # Main server file with Socket.IO logic
├── src/               # Frontend source code
│   ├── app/           # Next.js app directory
│   ├── components/    # React components
│   ├── contexts/      # React contexts
│   └── types/         # TypeScript type definitions
```

## 📝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 🙏 Acknowledgments

- Inspired by classic word-association board games
- Built with ❤️ by Pedro Barretto
