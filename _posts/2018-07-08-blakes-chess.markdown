---
title: "Blake's Chess"
layout: post
date: 2018-07-08 12:48
image: /assets/images/markdown.jpg
headerImage: false
tag:
- chess
- cards
- poker
- games
category: blog
author: thecharlesblake
description: A new chess variant using dice and playing cards
# jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f35c.png" height="20" width="20" align="absmiddle">'
---

## Requirements
- A chess set
- A deck of playing cards (no jokers)
- Two dice

## Setup & Gameplay

- Place only the kings and pawns on the board
- White to move first
- Cut the deck to determine which suit is _trumps_
- Shuffle the deck and place it face down (the _stock_ pile)
- All regular chess moves apply except:
  - There is no such thing as _check_. To win, one must capture the opposing king
  - When a piece goes to capture another piece, they must roll to determine whether the capture is successful (see [Capturing](#Capturing))
- For the first 3 turns, only regular moves and captures can be made
- After this, a player may instead draw a card (see [Drawing](#Drawing))
- A player may only play cards on their turn, and before their move (see [Playing Cards](#Playing Cards))

## Capturing

On their turn, if a player wishes to capture an opposing piece, they must first declare their intention to do so. Then each player must roll the dice to help determine their respective _attack_ and _defence_.

For a defending player, their _defence_ is the sum of their roll, and their _piece strength_. For the attacking player the calculation is the same, but they add 2 to their score as an _attack bonus_.

### Piece strengths
- __Pawns:__ 0
- __Knights:__ 1
- __Bishops:__ 2
- __Rooks:__ 3
- __Queens:__ 4
- __Kings:__ 5

Whichever player's total is higher captures their opponent's piece. Successful attacking pieces move onto the defender's square, whereas successful defending pieces remain in place. In the event of a draw, both pieces remain in place and the turn ends.

## Drawing

On their turn a player may draw a single card as an alternative to moving or capturing. Cards may either be drawn from the top of the _stock_ pile or the _waste_ pile (a second face-up pile next to the stock). A drawn card may be held indefinitely in a player's _hand_.

However, hands are limited to a maximum of 5 cards. If a player wishes to draw a card when they have reached their maximum hand size, they may do so, but upon drawing must immediately discard a card from their hand (including the one just drawn) and place in on top of the waste pile.

If the stock pile is exhausted, the waste must be shuffled, turned over, and becomes the new stock pile.

## Playing Cards
Before a player moves or attempts a capture, they may play a card or group of cards from their hand. Certain cards / groups of cards have particular effects on the game. These are broken down into two categories: __poker hands__ and __trump cards__. Poker hands and trump cards may be played in combination, and there is no limit to the number that a player may play on their turn. The effects of a card / group take place once on the turn they are activated.

Note that a card may be played on the same turn it is drawn. Played cards or groups of cards are placed on top of the waste pile in any order once their effect has taken place.

 The effects of these cards are as follows:

### Poker Hands

- __2 pair:__ +1 to any roll
- __3 of a kind:__ +2 to any roll
- __4 of a kind:__ +3 to any roll
- __3 card straight:__ Build first knight / bishop / rook (see [Building Peices](#Building Pieces))
- __4 card straight:__ Build the queen
- __5 card straight:__ Build all remaining pieces at once
- __3 card flush:__  Build second knight / bishop / rook
- __4 card flush:__ Build the queen
- __5 card flush:__ Select any opposing piece (excluding the king) to be removed from play
- __Kings:__ Blocks an attack on the king
- __Queens:__ Blocks an attack on the queen
- __Jacks:__ Blocks an attack on any other piece

Note that all cards which add to rolled values are to be played _after_ the dice has been rolled.

### Trump Cards
A: swap two opponent pieces (excluding king) and end turn,
2: move through one of your own pieces
3: double-agent-pawn: take-over an enemy pawn for a turn (attacks in your direction of movement)
4: board-wrap,
5: teleport any piece and end your turn,
6: sniper (can't die one's-self),
7: double-move,
8: bodyguard: swap a piece that is about to die with a pawn to take its place (excluding king)
9: two pieces attack at once (combine attack bonus, choose a piece to move in/die)
10: kamikaze (+2 attack bonus),
J: bishop converts (if possible),
Q: lowest attack wins (except for kings),
K: revive one of your dead pieces

## Building Pieces
