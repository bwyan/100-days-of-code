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

### Day 9: January 11, 2017

**Today's Progress**: I cleaned up the JS and continued work on my sequence player for the Simon game.

**Thoughts:** I coded at lunch and on the bus home, and wasn't nearly as productive as working in my office at home. I'd rather put some focused time in at home in the future vs trying to squeeze it in here and there.

**Todo:**
Tomorrow
- [ ] Finish the sequence playback in JS so that the notes don't all play at once (hopefully for real this time).

Future
- [ ] Work on the game logic in JS.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.

**Link to work:** [Free Code Camp – 2017-01-11 – Simon](https://codepen.io/bwyan/full/jyPVBy/)

### Day 10: January 12, 2017

**Today's Progress**: I got my sequence player to work, so now I can pass an array of pad numbers and have the computer play them back. You can try it yourself by clicking the start button.

- [x] Finish the sequence playback in JS so that the notes don't all play at once (hopefully for real this time).

**Thoughts:** I'm happy I got the app to play back a sequence, but I'm not happy with the timing of the audio playback. Sometimes a few notes are clustered together, and other times there's a gap larger than the duration I've passed to `setInterval`. I used data URIs in place of external URLs, which helped reduce the lag from loading, but there's more I need to do to get reliable and fast playback.

**Todo:**
Tomorrow
- [ ] Hook up the playback events to the UI so that the board lights up when the sounds play.

Future
- [ ] Work on the game logic in JS.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.
- [ ] Tweak the sequence player to improve its timing.
 
**Link to work:** [Free Code Camp – 2017-01-12 – Simon](https://codepen.io/bwyan/full/Grqgvr/)

### Day 11: January 13, 2017

**Today's Progress**: 

- [x] Hook up the playback events to the UI so that the board lights up when the sounds play.

**Thoughts:** I'm happy I got the app to play back a sequence, but I'm not happy with the timing of the audio playback. Sometimes a few notes are clustered together, and other times there's a gap larger than the duration I've passed to `setInterval`. I used data URIs in place of external URLs, which helped reduce the lag from loading, but there's more I need to do to get reliable and fast playback.

**Todo:**
Tomorrow
- [ ] Try MIDI.js to replace the poorly timed audio events, or look for another option.
- [ ] Implement a better option to improve audio event timing.

Future
- [ ] Work on the game logic in JS.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.
- [ ] Tweak the sequence player to improve its timing.
 
**Link to work:** [Free Code Camp – 2017-01-13 – Simon](https://codepen.io/bwyan/full/EZyENw/)

### Day 12: January 14, 2017

**Today's Progress**: Today I learned about the Web Audio API and created a simple sound player. Due to XHR/CORS issues I once again added the sounds as base64 URIs instead of URLs.

**Thoughts:** The Web Audio API gives my audio geek side a chance to really shine, but even better is it's the solution to my playback timing woes. Before integrating today's work into my Simon game, I'm going to try using oscillators instead of audio files. I think it will make the game more Simon-like, and allow the sounds to work better as the playback rate increases.

**Todo:**
Tomorrow
- [ ] Create a demo app where I try Web Audio API oscillators in place of audio files.

Future
- [ ] Work on the game logic in JS.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.
 
**Link to work:** [Free Code Camp – 2017-01-13 – Simon](https://codepen.io/bwyan/full/EZyENw/)

### Day 13: January 15, 2017

**Today's Progress**: Today I built a simple "instrument" with the Web Audio API. It has two buttons and each has a different sound.

**Thoughts:** This is the system I'll add to my Simon game tomorrow, for the reasons I mentioned in yesterday's log.

**Todo:**
Tomorrow
- [ ] Replace `<audio>` elements in my Simon game with web audio oscillators.

Future
- [ ] Work on the game logic in JS.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.
- [ ] Tweak the sequence player to improve its timing.
 
**Link to work:** [Web Audio API Test](https://github.com/bwyan/100-days-of-code/blob/master/oscillator.html)

### Day 14: January 16, 2017

**Today's Progress**: Today I built a sequencer into my Simon game, using the Web Audio API. It is not elegant and doesn't work on touch devices, but it's a start.

**Thoughts:** I have tons of repeating code so I'll be refactoring for a bit. The actual sequencer still uses `setTimout` instead of taking advantage of the web audio API, but I'm generating sound in the browser (really cool!) and my timing issues are fixed!

**Todo:**
Tomorrow
- [ ] Remove the code that was playing audio files.
- [ ] Add a proper sequencer using Web Audio API events.
- [ ] Get it working on iOS and Android.

Future
- [ ] Work on the game logic in JS.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.
- [ ] Tweak the sequence player to improve its timing.
 
**Link to work:** [Free Code Camp – 2017-01-16 – Simon](https://codepen.io/bwyan/full/ygVYve)

### Day 15: January 17, 2017

**Today's Progress**: Today I tried to build a Voice to replace my individual routines for building voices. I got hung up on how to initialize the oscillators from within `Voice`, so I wasn't able to complete my task. I will try again tomorrow with another approach.

**Thoughts:** I thought I had a good grasp on ES5 "classes", but I tried using ES6 class syntax and couldn't make it work. Bummer…

**Todo:**
Tomorrow
- [ ] Remove the code that was playing audio files.
- [ ] Add a proper sequencer using Web Audio API events.
- [ ] Get it working on iOS and Android.

Future
- [ ] Work on the game logic in JS.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.
- [ ] Tweak the sequence player to improve its timing.
 
**Link to work:** [Free Code Camp – 2017-01-16 – Simon](https://codepen.io/bwyan/full/ygVYve)

### Day 16: January 18, 2017

**Today's Progress**: Today I almost took the day off because I was so frustrated by yesterday's lack of progress. Instead I started with some easy code cleanup and writing helper functions like `addToCPUSequence()`. Before I knew it, I had built a good chunk of the game code, added a gap between notes in the sequencer, and more.

**Thoughts:** This goes to show the importance of showing up every day and forcing myself to code even when I don't feel like it (or is it *especially* when I don't feel like it). I made a lot of progress and it makes me excited to continue tomorrow instead of dreading the possibly of another unproductive coding session.

**Todo:**
Tomorrow
- [ ] Finish the game logic: enforce strict mode, add the counter, speed up playback after 5 pads are played.

Future
- [ ] Disable click handlers while the sequence is playing.
- [ ] Get it working on iOS and Android.
- [ ] Add a proper sequencer using Web Audio API events.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.
 
**Link to work:** [Free Code Camp – 2017-01-18 – Simon](https://codepen.io/bwyan/full/wggmQO)

### Day 17: January 19, 2017

**Today's Progress**: I finished everything I set out to do yesterday.

- [x] Finish the game logic: enforce strict mode, add the counter, speed up playback after 5 [also 9 and 13] pads are played.

**Thoughts:** 

**Todo:**
Tomorrow
- [ ] Remove a couple of quick 'n dirty uses of jQuery so everything is vanilla JS.
- [ ] Disable click handlers while the sequence is playing.

Future
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.
- [ ] Get the buttons working on iOS and Android.
- [ ] Add a proper sequencer using Web Audio API events.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
 
**Link to work:** [Free Code Camp – 2017-01-19 – Simon](https://codepen.io/bwyan/full/wggmQO)

### Day 18: January 20, 2017

**Today's Progress**: I finished everything I set out to do yesterday.
- [x] Remove a couple of quick 'n dirty uses of jQuery so everything is vanilla JS.
- [x] Disable click handlers while the sequence is playing (sort of).
- [x] Get the sound working on iOS.

**Thoughts:** I disabled the click handlers that track user input and could interfere with gameplay, but it's possible to play sounds while Simon is playing a sequence. Disabling click handlers (actually `mousedown` and `touchstart` events) for the synth and visuals would require a ton of unnecessary copy and pasting unless I refactor the synth code. For now it's okay as-is I might return to do some cleanup once I'm to the polishing stage.

**Todo:**
Tomorrow
- [ ] Add the light over the strict mode button.
- [ ] Add an on/off switch.
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.

Possible Future Improvements
- [ ] Add a proper sequencer using Web Audio API events.
- [ ] Test on Android and Windows.
 
**Link to work:** [Free Code Camp – 2017-01-20 – Simon](https://codepen.io/bwyan/full/wggmQO)

### Day 19: January 22, 2017

**Today's Progress**: I added the light over the strict mode button and cleaned up some code here and there. I also added a Web Font from Adobe Edge.

**Thoughts:** I probably spent more time looking for alternative to Google Fonts than I did coding, but it was still pretty fun.

**Todo:**
Tomorrow
- [ ] Finish styling the controls: Counter, start button, strict mode toggle.
- [ ] Start my portfolio page.

Possible Future Improvements to Simon.
- [ ] Add an on/off switch.
- [ ] Add a proper sequencer using Web Audio API events.
- [ ] Test on Android and Windows.
 
**Link to work:** [Free Code Camp – 2017-01-22 – Simon](https://codepen.io/bwyan/full/wggmQO)

### Day 20: January 23, 2017

**Today's Progress**: I got a lot done tonight

- [x] Finished the remaining user stories for my Simon game and added some extra flair.
- [x] Fixed up my older projects, which had broken since 18 months ago due to changes in the APIs.
- [x] Double-checked that I wasn't missing any user stories in my older projects.

**Thoughts:** I'm just one algorithm and a simple portfolio page away from completing my Front End development certificate. There's no reason I can't do it by Wednesday.

**Todo:**
Tomorrow
- [ ] Do the last @FreeCodeCamp algorithm challenge.
- [ ] Finish my portfolio page.
- [ ] Submit my Front End projects for final review!

**Link to work:** [Free Code Camp – 2017-01-23 – Simon](https://codepen.io/bwyan/full/wggmQO)

### Day 21: January 24, 2017

**Today's Progress**: I worked on my portfolio page and discovered I do not like writing about myself.

**Thoughts:** The writing took longer than I thought. I'm hoping to add the images, give it some polish, and wrap up by the end of the week.

**Todo:**
- [ ] Do the last @FreeCodeCamp algorithm challenge.
- [ ] Finish my portfolio page.
- [ ] Submit my Front End projects for final review!

**Link to work:** [Free Code Camp – Portfolio](https://codepen.io/bwyan/full/OyJaoz/)

### Day 22: January 26, 2017

**Today's Progress**: I worked on my portfolio page some more. Got the assets posted on GitHub and tweaked the thumbnail styling. I wrestled for a while with the thumbnail not wrapping properly and didn't resolve it.

**Thoughts:** In the original FCC curriculum (when I started this portfolio), it was required to use Bootstrap. I'm not enjoying the amount of nested `div` elements needed to make it work though, and without writing the CSS myself, it's hard to diagnose problems like the one I had with wrapping.

**Todo:**
- [ ] Do the last @FreeCodeCamp algorithm challenge.
- [ ] Finish my portfolio page.
- [ ] Submit my Front End projects for final review!

**Link to work:** [Free Code Camp – Portfolio](https://codepen.io/bwyan/full/OyJaoz/)

### Day 23: January 27, 2017

**Today's Progress**: Boom!

- [x] Do the last @FreeCodeCamp algorithm challenge.
- [x] Finish my portfolio page.
- [x] Submit my Front End projects for final review!
- [x] Get my Front End dev certificate!!!

**Thoughts:** I figured out the problems with my thumbnail gallery by (drum roll…) reading the documentation!! Turns out I needed a couple of divs to help with the spacing issues. I'm still not a fan of all the `div` elements that Bootstrap needs, but it got the job done for this.

Also, this certificate was over two years in the making (one of them was a total hiatus, but the other was a lot of work). I'm proud of how much I learned from the projects and can't wait to start the React/Data Vis cert. I've debated spending more time tweaking the projects I've already done so they look nicer, but I'm so eager to move on and challenge myself with new things, rather than just play with the same code all over again.

**Todo:** Start the Data Vis certification with Wes Bos' React for Beginners course. I'll do just enough of the course to get started on the projects, and then focus 80% on the projects and 20% on the tutorials.


**Link to work:** [Free Code Camp – Portfolio](https://codepen.io/bwyan/full/OyJaoz/)

### Day 24: January 28, 2017

**Today's Progress**: I did the first 10 lessons in Wes Bos' React for Beginners course. It was a great update/refresher on React. A lot has changed since I toyed with it 18 months ago.

I also used create-react-app to set up a project for my Markdown Previewer.

**Thoughts:** I'm excited to be working with my own dev environments and moving away from Codepen for these projects. The learning curve is steeper, but I'm getting exposed to some great skills like working with npm and scripts.

**Todo:** Set up a GitHub repo for my Markdown Previewer, and clone it to my other computer.

**Link to work:** [bwyan/fcc-md-preview (GitHub)](https://github.com/bwyan/fcc-md-preview)

### Day 25: January 29, 2017

**Today's Progress**: I set up a GitHub repo for my Markdown project, added the two React components I'll need, and got the project working on my other computer.

I tried to eject the project to get Sass working, but I must have done something wrong because my css wasn't loading once I built the project.

**Thoughts:** It was really empowering to push a project to GitHub, clone it on another machine, and install all of the dependencies, all wihout referencing any documentation. I'm getting the hang of this and it feels great.

**Todo:** 

- [ ] Add event listeners to my `<TextInput>` component that push the text into the `<Preview>` component.
- [ ] Add marked.js to the project.
- [ ] (if time allows) get marked.js to interpret markdown and put html into the `<Preview>` component.

**Link to work:** [bwyan/fcc-md-preview (GitHub)](https://github.com/bwyan/fcc-md-preview)