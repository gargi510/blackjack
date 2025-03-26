# Blackjack Game in Python

## Description
This is a simple command-line version of the Blackjack card game built using Python. The game allows the user to play against the computer (dealer) by drawing cards and trying to reach a sum of 21 without exceeding it.

## Features
- Player vs Dealer gameplay.
- Ability to draw additional cards or pass.
- Card values:
  - Number cards (2-10) represent their face value.
  - Jack, Queen, King all have a value of 10.
  - Ace can be 1 or 11, depending on the player's hand.
- The game displays the player's hand, current score, and the dealer’s first card.
- The game checks for winners and losers based on the rules of Blackjack.

## Technologies Used
- Python 3.x
- `random` module for generating random card values.
- `replit` module for clearing the screen during gameplay.
- `art` module to display a logo.

## Installation

To run this project locally:
1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/blackjack-game.git
    ```

2. Install the required dependencies:
    ```bash
    pip install replit art
    ```

3. Run the script:
    ```bash
    python blackjack_game.py
    ```

## Gameplay Instructions
1. When you run the script, the dealer's first card will be revealed, and you will be given two cards.
2. You can choose to draw another card by typing `'y'` or pass by typing `'n'`.
3. The goal is to reach a hand value of 21 or as close as possible without exceeding it.
4. The dealer will draw cards until their hand value is at least 17.
5. Once the game ends, the results will be displayed, indicating whether you won, lost, or drew with the dealer.

## Code Overview
- **`generate_card(set)`**: Randomly selects a card from the deck and adds it to the given set (player's or dealer's hand).
- **`ace(cards)`**: Adjusts the Ace value if the total exceeds 21.
- **`check(user, dealer, cards)`**: Compares the player's hand with the dealer’s and announces the result.
- **`deal_(user_cards, dealer_cards)`**: Handles the player's decision to draw a card.
- **`pass_(user_cards, dealer_cards)`**: Handles the player's decision to pass and reveals the dealer’s final hand.
- **`blackjack()`**: Main function to run the game, allowing the player to make decisions and displays the game's state.

## Sample Output

```
Welcome to Blackjack!
Your cards: [10, 8], current score: 18
Computer's first card: [6]
Type 'y' to get another card, type 'n' to pass: y
Your cards: [10, 8, 4], current score: 22
You lose
Do you want to play a game of Blackjack? Type 'y' or 'n': n
Goodbye! Thank you for playing!
```

