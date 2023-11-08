# Tic Tac Toe Game

This project is built using React and demonstrates the use of hooks such as useState. it is a [tutorial](https://react.dev/learn/tutorial-tic-tac-toe) to learn **React** and improve my skills in react.

## Features

- **Innteractive Gameplay**: The game allows two players to play Tic Tac Toe interactively.

- **Game History**: The game keeps track of the entire history of the game allow players to navigate to previous moves freely.

  ![](/src/screenshots/game%20history.png).

- **Game Status Updates**: The game provides real-time status updates and shows which player's turn it is and who the winner is.

  ![](/src/screenshots/game%20status.png)

## Instruction to Run the project

1. clone the repo to your device.
2. Navigate to the project directory.
3. Install the necessary depencies by npm install.
4. Start the project by npm start.
5. Open[http://localhost:3000](http://localhost:3000) to view in the browser.

## Code Snippet

Here is a snippet from the code that handles the logic for a player's move:

```jsx
function handleClick(i) {
  if (calculateWinner(squares) || squares[i]) {
    return;
  }
  const nextSquares = squares.slice();
  if (xIsNext) {
    nextSquares[i] = "X";
  } else {
    nextSquares[i] = "O";
  }
  onPlay(nextSquares);
}
```

This function updates the state of the game board and determines next player.

## Screenshots

![](</src/screenshots/Screenshot(4).png>).

---

![](</src/screenshots/Screenshot(3).png>)
