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

### Day 4: January 6, 2017

**Today's Progress**: Started the HTML and CSS for my next Free Code Camp project: a Simon game:

* Four buttons with different colors.
* Each button fills 1/4 of the screen.
* Clicked/pressed state.

**Thoughts:** I decided to try building the layout with flexbox, and was really happy with how simple it was. I would need to learn how to support older browsers if this were a production app, but as a project, it's fun to try the latest and greatest.

**Todo:** Add the other UI elements that are needed: Counter, start button, strict mode toggle, off/on switch.

Once that's done, I'll start bulding the game logic in JS.

**Link to work:** [Free Code Camp – 2017-01-06 – Simon](https://codepen.io/bwyan/full/jyPVBy/)

### Day 5: January 7, 2017

**Today's Progress**: Worked on styling for my Simon game. The board is now round and responsive, and there's a pad in the center for the center.

**Thoughts:** At some sizes, there's a small hairline between buttons that started appearing once I centered the settings-container. I would like to figure out how to make that hairline go away.

**Todo:** Add the other UI elements that are needed: Counter, start button, strict mode toggle, off/on switch.

Once that's done, I'll start bulding the game logic in JS.

**Link to work:** [Free Code Camp – 2017-01-07 – Simon](https://codepen.io/bwyan/full/jyPVBy/)

### Day 6: January 8, 2017

**Today's Progress**: Worked on Simon:

* New colors and tweaked gradients.
* Clicking the pads now plays audio (haven't tested on touch devices).
* I worked on some HTML for the other controls, but I've hidden them from today's share until they're finished.

**Thoughts:** Having fun doing this project with vanilla JS only.

**Todo:** Finish the other controls: Counter, start button, strict mode toggle, off/on switch.

Once that's done, I'll start bulding the game logic in JS.

**Link to work:** [Free Code Camp – 2017-01-08 – Simon](https://codepen.io/bwyan/full/jyPVBy/)

### Day 7: January 9, 2017

**Today's Progress**: Worked on Simon:

* Finished the layout for the counter, start button, and strict button.
* Adjusted some metrics for a nicer look at very small and very large screen sizes.
* I started work on the on/off switch, but it's not included in today's share.

**Thoughts:** I was hoping to get the controls built more quickly and then start the JS tomorrow, but I ran into a snag with the layout tonight. It looks like I'll need another day on the UI.

**Todo:**
Tomorrow
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.

Future
- [ ] Work on the game logic in JS.

**Link to work:** [Free Code Camp – 2017-01-09 – Simon](https://codepen.io/bwyan/full/jyPVBy/)

### Day 8: January 10, 2017

**Today's Progress**: I took a break from CSS and started working on sequence playback in JS.

**Thoughts:** I need a polyfill for the `.click()` method (vanilla JS, not jQuery) that works on mobile devices.

I struggled to get `setInterval()` or `setTimeout()` working with my sequence player, so I'll have to figure that out before moving on. I'm starting to think that writing the actual game logic will be easier than getting the basic methods done.

**Todo:**
Tomorrow
- [ ] Finish the sequence playback in JS so that the notes don't all play at once.

Future
- [ ] Work on the game logic in JS.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.

**Link to work:** [Free Code Camp – 2017-01-10 – Simon](https://codepen.io/bwyan/full/jyPVBy/)