# ♟ Chess.com Clone

A multiplayer, browser-based chess game built using **Node.js**, **Express**, **Socket.IO**, and **Chess.js**. This clone allows two players to connect and play live chess games, while spectators can observe in real time.

---

## 🚀 Features

- 🔁 Real-time multiplayer chess via WebSockets
- ♟ Interactive drag-and-drop chessboard using Unicode characters
- 👥 Player assignment: white, black, or spectator
- 🎮 Legal move validation via the `chess.js` library
- 🖥️ Responsive 8x8 chessboard with Tailwind CSS
- 🛑 Game-over detection
- 🔄 Automatic board flipping for black player

---

## 🛠 Tech Stack

| Layer     | Technology          |
|-----------|---------------------|
| Frontend  | HTML, CSS, Tailwind, EJS, Vanilla JS |
| Backend   | Node.js, Express    |
| Real-time | Socket.IO           |
| Game Logic| [chess.js](https://github.com/jhlywa/chess.js) |

---

## 📂 Folder Structure

chess.com-clone/
├── public/
│ └── js/
│ └── chessgame.js # Frontend logic (drag-drop, rendering, Socket.IO)
├── views/
│ └── index.ejs # HTML template rendered by Express
├── app.js # Main server with Socket.IO and Express
├── package.json


---

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/dpbd-2004/chess.com-clone.git
   cd chess.com-clone

## Install dependencies
npm install

## Start the development server
node app.js

## Visit
http://localhost:3000


## 👨‍🎓 How It Works

On connection:

First player becomes White

Second player becomes Black

Additional users become Spectators

Board state syncs via Socket.IO events:

"move": Broadcasts a valid move to all clients

"boardState": Updates full board using FEN

"playerRole" / "spectatorRole": Assigns user role

Chess logic handled by chess.js to ensure valid movement, captures, promotion, and game-ending conditions.

## 📷 Screenshot
![image](https://github.com/user-attachments/assets/e90c54ef-fee6-480b-bca3-cbb1be84a13f)

## 📌 Future Improvements

Add game timer (blitz, bullet, etc.)

Track and display move history

Allow player usernames and matchmaking

Support draw/resign/game reset

Deploy to Vercel or Heroku

## 📝 License

This project is open-source and available under the MIT License.


