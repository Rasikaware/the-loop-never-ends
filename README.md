# Retro Game Box (SEDA Project SuSe2026)
**Team: Loop Never Ends**

A collection of retro-style multiplayer games built with JavaFX, featuring a Memory Game, Tetris battle and Chess.

## Prerequisites
- **Java 21** or newer
- **Maven 3.8+**
- Local Area Network (for LAN multiplayer)

## Build & Run
```bash
# Compile and run via Maven
mvn clean compile
mvn javafx:run
```

---

## 1. Memory Game
A classic card matching game with LAN support and configurable difficulty.

### Features
- **Configurable Match Size (n):** Match 1 to 45 cards of the same kind.
- **Dynamic Deck Size:** Adjust the total cards in play (must be divisible by n).
- **Pokemon Theme:** Custom card assets and glassmorphic UI effects.
- **LAN Multiplayer:** Sync state, scores, and turns across two machines.

### Gameplay
- Player 1 (Host) sets the match size and deck size.
- Players take turns flipping **n** cards.
- If all match, you score a point and keep your turn.
- If they don't match, cards flip back and the turn passes.

---

## 2. Tetris
A 1v1 Tetris variant where two players play on the same screen or over LAN.

### Features
- **Dual-Board Layout:** Player-1 at the bottom, Player-2 at the top.
- **Swap Power-up:** Clearing lines spawns magenta "Swap" icons. Touching them swaps both players' boards instantly.
- **Custom Piece Designer:** Build your own tetrominoes and use them in the game.
- **Piece Preview:** Preview of the next piece.
- **LAN Support:** Host a session or scan for active hosts on your network.
  **Horizontal Play:** You can play in horizontal mode as well.

### Controls
| Action | Player 1 (Bottom Board) | Player 2 (Top Board / Client) |
| :--- | :--- | :--- |
| **Move** | Arrow Keys Left / Right | A / D |
| **Soft Drop** | Arrow Down | W |
| **Hard Drop** | Space | Left Shift |
| **Rotate CW** | Arrow Up | S |
| **Rotate CCW** | Z | Q |

---

## Networking Notes
- **Hosting:** Click "Host Game" to start a server on port **28080**. Your IP will be displayed.
- **Joining:** Click "Join Game". You can either type the IP manually or use the "Scan for LAN Hosts" feature to find active games on your network automatically.

## 3. Hexagonal Chess
A Gliński’s variant of hexagonal chess. Where you have the option to play 1v1 on the same device, Host a game or Join a game over the same
LAN session, play with computer or design your board. 

### Features

**Hexagonal Layout:** Not like the classic chess, but with a twist of variations, and movement of the chess pieces.
**LAN Support:** Host a Chess game on your device, or join a game using the IP Address and Port number over a LAN.
**Play 1v1:** Play with a person on a same device turn by turn.
**Play with the computer:** You have option to play with computer as an opponent.
**Custom Chess Baord Designer:** You can design a chess board, with the pieces of your choice however you want to make it fun and interesting.

