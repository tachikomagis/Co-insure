# Automonous World Hackson, proposal 

## Brief
Multiplayer Pong War

Pong War: (Original?)
https://github.com/vnglst/pong-wars

## Game Type
2D, Multiplayer, Strategy

## Engine
https://github.com/vocdex/pong-wars-python
Based on the this python version

※ As an online version may need quite some time to deal with the P2P and sync parts, we may just make an offline version (with buttons for pausing the game and changing players) first.

As future work, an online version, as well as an on-chain version, could be expected.
(Maybe made by others, though)

## Concept
Instead of just watching, players can affect the wars actively in our game.
Each player has his/her initial points, and they can use them to "buy" other players' area. Of course, other players can also refuse to sell it, by paying more points.
The one with the most points (the sum of points they have and the blocks they finally get), will be the winner.

What's more, the players could be different from each other by being able to choose from several types, e.g. some type could have a somehow faster ball and a smaller initial area, another type could have different shape of area that they can buy.
And the type could be like...countries.
This could be the +alpha part of this game, need to be detailed later.

## Details
(All the numbers are just examples, could be changed during the development)

### Common parts
0. Each player chooses his/her color, and gets a initial 100 * 100 area, with 1000 points.
1. Pong wars start.
2. When someone wants to buy areas, he/she clicks the "Pause" button, change the operator to his/her player by clicking button.
3. Then he/she needs to choose the size of area that he/she wants to buy, from "5 * 5" and "10 * 10", also the coordination of the area.
(The trade will be applied to all players)
4. The cost is the size of area * number of players. Notice that it is the size the player chose, rather than the blocks he/she actually brought.
(For example, even some of the areas that he/she buys already him/hers, he/she still needs to pay for it. The cost is for the trade itself rather than the blocks)
5. Other players can refuse this trade, by paying twice of the point, for the size of the area in his/her part.
(Neither the pay nor the cost will be got by the players, they just vanish)
6. After like 5min, or some player died? (blocks less than like...10?), the game ends. The one having the most blocks + points is the winner.

Three modes are provided: 1v1, 2v1, 1v1v1v1

About the 2v1 part, one has 200 * 100 area from the start, with some disadvantage maybe.
(Need to be detailed later)


## Notice
Still not know whether the game will be interesting or not, and what the balance will be like.
Need to make it out first and then think about what needs to be change later.
