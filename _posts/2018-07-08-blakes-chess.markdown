---
title: "Blake's Chess"
layout: post
date: 2018-07-08 12:48
image: /assets/images/chess.png
headerImage: true
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

The following is a set of rules for a game I have invented, which I'm
provisionally calling _Blake's Chess_ (where's the fun in being a narcissist if
you don't get to name things after yourself?). This variant is inspired by the
idea of turning chess into an imperfect-information game, where probability and
chance are introduced.

The game is really a variant of chess with the attacking dynamics of _Risk_,
and a set of _effect cards_ as found in many popular board games,
but based on poker hands formed by playing cards.

Many chess variants [already exist][1], and are widely played. Additionally, some of
these mechanics have been experimented with before in relation to chess (see
[Knightmare Chess][4], [Fantasy Chess][3], and [ChessHeads][2]).
However, _Blake's Chess_ is quite distinct from these other games and is unlike
anything I'm currently aware of.

The game is still a work-in-progress. Please forgive any warped game mechanics.
Feedback is always appreciated :)

<div class="img_container" style="text-align: center;">
<img src="/assets/images/strategy.png" height="240px"/>
</div>

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
  - When a piece goes to capture another piece, they must roll to determine whether the capture is successful (see [Capturing](#capturing))
- For the first 3 turns, only regular moves and captures can be made
- After this, a player may instead draw a card (see [Drawing](#drawing))
- A player may only play cards on their turn, and before their move (see [Playing Cards](#playing-cards))

<div class="img_container" style="text-align: center;">
<img src="/assets/images/board.png" height="240px"/>
</div>

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

Whichever player's total is higher captures their opponent's piece. Successful attacking pieces move onto the defender's square, whereas successful defending pieces remain in place. In the event of a draw, no capture takes place. Both pieces remain in place and the turn ends.

<div class="img_container" style="text-align: center;">
<img src="/assets/images/dice.png" height="240px"/>
</div>

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
- __3 card straight:__ Builds the first knight / bishop / rook (see [Building Peices](#building-pieces))
- __4 card straight:__ Builds the queen
- __5 card straight:__ Builds all remaining pieces at once
- __3 card flush:__  Builds the second knight / bishop / rook
- __4 card flush:__ Builds the queen
- __5 card flush:__ Selects any opposing piece (excluding the king) to be removed from play
- __Kings:__ Blocks an attack on the king
- __Queens:__ Blocks an attack on the queen
- __Jacks:__ Blocks an attack on any other piece

Note that all cards which add to rolled values are to be played _after_ the dice has been rolled.

<div class="img_container" style="text-align: center;">
<img src="/assets/images/cards.png" height="240px"/>
</div>

### Trump Cards

These card ranks refer to the cards in the deck whose suit matches the card
selected as the _trump_ card at the beginning of the game.

- __A (misdirection):__ Swaps two of your opponent's pieces (excluding the king)
- __2 (invisibility):__ Enables you to move a piece through other pieces of your own, as though they
  were not there, as long as the move would otherwise be valid and no two pieces
  finish on the same square
- __3 (brainwashing):__ Takes-over an enemy pawn for a turn. It moves and attacks in your own
  direction of play
- __4 (secret passageway):__ Allows moves to wrap width-wise, such that a piece may
  make a legal move out the left side of the board and finish on the right (or
  vice-versa)
- __5 (teleportation):__ Moves one of your pieces (excluding pawns) to any other empty square and ends your turn
- __6 (sniper):__ An attack on an opposing piece, does not move to their square if
  successful. The attacking piece is also not captured if unsuccessful
- __7 (agility):__ Allows two moves/captures/draws on this turn
- __8 (bodyguard):__ Swaps a piece that is about to die (excluding the king) with any other piece to take its place
- __9 (tag-team):__ Two pieces may attack at once, combining their piece strength. One piece is
selected beforehand to move to the target square if successful. Both attacking pieces are captured if
unsuccessful
- __10 (kamikaze):__ Grants a piece an extra 2 points for an attack, but the
  piece is automatically captured whether it wins or loses
- __J (conversion):__ A bishop that successfully captures a piece which you have
  either lost or not yet acquired, instead converts that piece into one of your
  own
- __Q (uprising):__ Swaps the piece strength of the attacking and defending
  pieces (excluding defending kings)
- __K (necromancy):__ Revives one of your dead pieces

## Building Pieces

There is an order in which pieces must be built. Firstly, a rook, a knight and a
bishop must be built (in any order). After these three have been completed, a
queen must be built. Finally the second rook, knight, and bishop must be built
(again, in any order).

Pieces may only be built if they have not been built before. Captured pieces may
not be rebuilt.

[1]: https://en.wikipedia.org/wiki/List_of_chess_variants
[2]: https://www.boardgamegeek.com/boardgame/12932/chessheads
[3]: http://www.shadowhex.com/
[4]: https://en.wikipedia.org/wiki/Knightmare_Chess
