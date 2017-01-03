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
