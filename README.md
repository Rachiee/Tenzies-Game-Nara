# Tenzies Game

A React implementation of the classic Tenzies game. Roll the dice until all values match, and strategically hold specific dice to reach the winning combination.

## Features

* Ten dice that can be rolled, held, and reset
* Win detection when all dice show the same value and are held
* Automatic focus on the New Game button after winning
* Confetti animation upon winning
* Screen reader friendly with ARIA live announcements

## How It Works

1. The game starts with ten randomly generated dice.
2. Each die has:

   * A value from 1 to 6
   * A held state
   * A unique ID for tracking
3. Players click on dice to toggle their held state.
4. Rolling updates only the unheld dice.
5. When all dice are held and share the same value, the game is won.
6. After winning, the roll button becomes a New Game button which resets the dice.

## Technologies Used

* React
* JavaScript (ES6)
* nanoid for unique IDs
* react-confetti for the win animation
* Custom CSS for styling

## Getting Started

### Prerequisites

* Node.js and npm installed locally

### Installation

1. Clone the repository
   `git clone <your-repo-url>`

2. Navigate to the project folder
   `cd your-project-folder`

3. Install dependencies
   `npm install`

4. Start the development server
   `npm start`

## Project Structure

* `App.jsx` contains the game logic, win detection, and dice rendering.
* `Die.jsx` is a reusable component representing an individual die.
* `index.js` renders the app to the DOM.
* `styles.css` controls layout and appearance.

## Game Rules

* Roll the dice repeatedly until all ten dice show the same value.
* Click a die to hold it so it does not change during rolls.
* Once all dice match and are held, you win and can start a new game.