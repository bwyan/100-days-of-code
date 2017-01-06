# 100 Days Of Code - Log

### Day 1: January 3, 2017

**Today's Progress**: Added a delay when the CPU takes a turn, to accomplish two goals:

* Build some suspense while the user waits for the CPU to move.
* I didn't like the CPU moving at essentially the same time as a human player, becuase it could be hard to see where the CPU moved most recently. The delay helps with this, and prevents the need for an animation, which could be distracting.

**Thoughts:** I added the delay easily with setTimeout(), but the board was still clickable, so it was possible to move for the computer. I added functions to lock and unlock the board, and call them at the beginning and end of the CPU's turn. 

This also let me pull the lock/unlock code out of other functions and replace it with a function call, so I got to do some refactoring too.

**Todo:**

* Continue refactoring and commenting, as the app is functionally complete but the code is messy. 
* Make it beautiful.
* Bonus: replace all uses of jQuery with vanilla JS.

**Link to work:** [Tic Tac Toe - 2017-01-03](https://codepen.io/bwyan/full/zNOapV/)

### Day 2: January 4, 2017

**Today's Progress**: Light refactoring and cleanup on my Tic Tac Toe game:

* Moved the unlockBoard() function call to the takeTurnWithAI() method.
* In the HTML, I replaced an ID with a data attribute, which is more appropriate for my click handler to use and let me remove a few lines of code. I learned that it's the more proper way to do what I wanted to do thanks to the first project in Wes Bos' "30 days of JS" videos.
* I made the Xs and Os bigger and the lines on the board thicker.

I also fixed a bug that caused the click handlers to return NaN sometimes.

**Thoughts:** I'm starting to try some ES6 features like template strings, which is quite fun. I might want to study up on workflows for refactoring, rather than wander through my code looking for opportunities.

**Todo:** Same as yesterday:

* Continue refactoring and commenting, as the app is functionally complete but the code is messy. 
* Make it beautiful.
* Bonus: replace all uses of jQuery with vanilla JS.

**Link to work:** [Tic Tac Toe - 2017-01-04](https://codepen.io/bwyan/full/Kawaab/)

### Day 3: January 5, 2017

**Today's Progress**: Light refactoring and cleanup on my Tic Tac Toe game:

* Replaced some instances of let with const.
* Re-ordered some of the code so similar functions were closer together.

Then, I spent quite a while on making the UI look nicer, including moving the scoreboard below the gameboard and tweaking the type styles, creating a dialog for the player and symbol choices (vs having them appear at the bottom of the screen), styling the choice buttons, etc.

Finally, I fixed a few bugs that could allow players to cheat if they are fast clickers and playing against the computer.

**Thoughts:** I took a needed break from refactoring, and will start on my next project (the Simon game) before spending more time on Tic Tac Toe.

**Todo:** Start working on Simon and take a break from Tic Tac Toe.

**Link to work:** [Tic Tac Toe - 2017-01-05](https://codepen.io/bwyan/full/QdwYwK/)