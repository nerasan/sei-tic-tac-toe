# Peudo-Code Tic Tac Toe

Next Week, you'll be building a [tic-tac-toe](https://en.wikipedia.org/wiki/Tic-tac-toe) game from scratch. To prepare, the deliverable this week is to plan it out! You'll also get to practice writing [markdown](https://guides.github.com/features/mastering-markdown/).

## The Assignment

Fork & Clone this repo. Open this file in your text editor and fill in the sections below. When you're done, make a pull request!

### Part 1: Make a To-Do list

Write out a list of *all* the things you need to do to code this game. This can be as detailed or high-level, though we recommend the former. This is your first time planning an app, so just have fun and just see what you can come up with. There's no right way.

---

Have the HTML, CSS, and JS files.
Make a layout of the website for the user to play tic-tac-toe.
Make it simple where it only has the game in the center (main focus of the site) and other details at the top (the score) and the sidebar (menu, settings, etc.).
Use appealing colors for the user to play.
Make it easy to understand how exactly to play -- for example, by simply clicking on where you want to place your move.
Allow the user to choose whether they want to be X or O.
Most of the functions will be in the JS file, including the event listeners when the user clicks. So the user clicking if they want to be X or O will prompt the game to continue with the user placing the character they chose.
Create a function that allows a computer to move based on the user's move and to invoke this after the user clicks to place their move.
When the user wins or loses, make it clear showing how the user or the computer won (by drawing a line through the three spots).
After a round, allow the user to continue another round or reset (resetting the score back to zero). Invoke the function back to the start of the game (resetting score to 0).
Have a count every time the user or computer wins and add by 1.
Sidebar menu should be minimal to not distract the user from the game.
Create a footer which includes links to the creator of the site.


---

### Optional Part 2: Pseudo-code your win-logic

Each time a player makes a move, your code will check to see if there is a game-over condition (a win or a draw). Write out this logic in english/psuedocode below. When you're done, anyone should be able to read your pseudo-code and translate it line-by-line into javascript or another language.

---

When a player makes a move (clicks somewhere in the grid), the code will check the following condition.
If the user has three moves in a row, then the user wins and the user's score increases by 1.
Else if the computer has three moves in a row, then the computer wins and the computer's score increases by 1.
Else the round resulted in a draw.
After this condition is checked, invoke the option for the user to play another round (invoke the function to start a new round) or reset the score (invoke the function to reset the score variable back to 0 and start a new round).

---

### Notes on Planning Tic-Tac-Toe

Gameboard
- 3x3 grid of divs
- reset button 

using id and class on clickable elements will help you wire it up in JS afterwards

JavaScript
- select elements and attach functions via event listeners
- variable to keep track of moves
- used to indicate whether or not to draw an x or an o -- same code amal used?

Requirements
- user can click on different squares to make a move -- similar to the changing shape exercise -- using event.target

- every click will alternate between marking x and o -- might be similar to amal's code? but might not need the counter++ maybe just set as 0 and 1 and have the if loop go back to if === 0 else if === 1. this would be nested in another if to test if any are in a row.

- upon marking individual cell, use JS to add a class to each cell to display the separate players -- mark as x or o

- a cell should not be able to be replayed once marked -- how to make it where the user can't click once a div already has a class of x or o?

- once game is over, you cannot click remaining empty cells -- kill the function?

- reset button will clear contents of the board -- clear and restart the game function

- display message to indicate which turn is about to be played

- detect draw conditions -- ties/cat's game?

- detect winner: stop game and declare winner if one player ends up getting three in a row -- will need to determine a set of winning combinations. check those combinations on the board contents after every move.

would it be a really nested if? can you put conditions in an array? yes... it is an option.
https://stackoverflow.com/questions/31604252/java-script-using-array-to-store-conditions


### PROGRESS -- to commit

8/16
set up html, css, js base to start game, reset button, and add event listeners to click O or X

8/19
redoing the grid container
data-cell-index
https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes