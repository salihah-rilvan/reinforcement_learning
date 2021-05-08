# reinforcement_learning
This repository features my code for a card game using the reinforcement learning concept

Here is the description:

Game is played with infinite deck of cards
Each draw from deck results in value between 1 and 10 (uniformly distributed) with a color
of red (probability 1/3) or black (probability 2/3)
At the start of the game both the player and dealer draw one black card

Each turn the player may either stick or hit
If player hits, then she draws another card from the deck
If player sticks, she receives no further cards
The value of players cards is added (black cards) or subtracted (red cards)
If player’s sum exceeds 21, or becomes less than 1, then she “goes bust” and loses the game
(reward -1)

If the player sticks, then the dealer starts taking turns. The dealer always sticks on any sum of
17 or greater, and hits otherwise. If the dealer goes bust, then the player wins; otherwise the
outcome-win (reward +1), lose (reward -1), or draw (reward 0) - is the player with the largest
sum.
1. Build a simulator that simulates the draw of cards and play of the game between
player and dealer.
2. Then, implement a Q-learning approach to maximize expected reward in this game
