---
layout: project
type: project
image: 
title: Rock, Paper, Scissors
permalink: projects/micromouse
# All dates must be YYYY-MM-DD format!
date: 2020-01-23
labels:
  - CSS
  - HTML
  - JavaScript
summary: I was trying out javascript by myself before class started, watched tutorials on how to make small games, this is what I made.
---



This program recreates the game rock, paper, scissors using HTML, CSS, and JavaScript. I was practicing coding during the last week of my winter break, I was watching youtuber "Clever Programmer" and his video was titled "JavaScript Tutorial for Beginners - Full Course in 8 Hours [2020]". The javaScript code is similar, but the HTML and CSS coding is different.

How the game works is you choose rock, paper, or scissors and your "opponent" chooses those three randomly, if both are the same you tie, if they are different then you either win or lose. There is also a button to challenge your opponent again. Things that I would like to add but not have time for it, is adding a score board, "battle" music, and animated images.

Here is some code that illustrates how the opponent chooses:

```js
function rpsGame(yourChoice) {
    console.log(yourChoice);
    let humanChoice, botChoice;
    humanChoice = yourChoice.id;

    botChoice = numberToChoice(randToRpsInt());
    console.log('Computer choice:', botChoice);

    results = decideWinner(humanChoice, botChoice); //Returns an array ex) [0, 1] = human lost
    console.log(results);

    message = finalMessage(results);
    console.log(message);
    rpsFrontEnd(yourChoice.id, botChoice, message);
}
```





