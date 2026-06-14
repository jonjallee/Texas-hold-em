#Texas Hold'em Poker Game

This repository features a terminal-based Texas Hold'em game written in Java, developed as a core course project for Java programming class.

>  **Acknowledgment:** Most of the architectural logic and algorithmic patterns within this project were developed with the collaborative assistance and technical guidance of Gemini.



##Key Features

* **Game Flow Control (`Phase`)**: Implements a complete Texas Hold'em cycle, spanning Pre-flop, Flop, Turn, River, and the final Showdown.
* **Modular Betting System (`BettingSystem`)**: Completely isolates input handling and chip pooling from the primary game loop to enforce proper object-oriented encapsulation.
* **Hand Evaluation (`Genealogy`)**: Uses an efficient array-frequency logic to systematically analyze 7 cards and rank combinations from Royal Flush down to High Card.
* **Opponent AI (`경주 이씨 한량`)**: Provides a dynamic, context-aware automated opponent to simulate authentic poker match-ups in the console.



##Class Architecture

* **`Main`**: Entry point handling configuration, string formatting, deck initialization (`Deck()`), and card consumption (`drawCard()`).
* **`Player` & `Table`**: State containers managing dynamic structural constraints—such as private/community card lists and active bet matching vectors.
* **`Phase` & `BettingSystem`**: Logical controllers running state loops and structural poker betting choices (Call / Raise / Fold).
* **`Genealogy`**: Evaluation module containing distinct poker hand ranking algorithms.
