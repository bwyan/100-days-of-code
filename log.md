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

### Day 26: January 30, 2017

**Today's Progress**: I needed to get the project setup to use Sass, so I started over with react-custom-scripts and create-react-app. Fixed up my github repo too, so everything is ready to start working again tomorrow. I made a few basic tweaks to the CSS just to make sure the scripts are all working correctly (they are).

**Thoughts:** Despite not getting any major progress done on the project itself, I'm really happy with my ability to read documentation, work with react-custom-scripts, and fix some issues I was having with my github repo getting out of sync between machines.

**Todo:** 

- [ ] Add event listeners to my `<TextInput>` component that push the text into the `<Preview>` component.
- [ ] Add marked.js to the project.
- [ ] (if time allows) get marked.js to interpret markdown and put html into the `<Preview>` component.

**Link to work:** [bwyan/fcc-md-preview (GitHub)](https://github.com/bwyan/fcc-md-preview)

### Day 27: January 31, 2017

**Today's Progress**: I finished the bulk of the Markdown Previewer project:

- [x] Add event listeners to my `<TextInput>` component that push the text into the `<Preview>` component.
- [x] Add marked.js to the project.
- [x] (if time allows) get marked.js to interpret markdown.
- [x] Add html-react-parser to put html into the `<Preview>` component with react elements instead of using `dangerouslySetInnerHTML`.

**Thoughts:** I always forget how much work there is to write CSS from scratch after a reset and not rely on browser defaults. The majority of my remaining work is going to be finishing the styling.

**Todo:** 

- [ ] Finish the CSS for all of the html elements that markdown supports.

**Link to work:** [bwyan/fcc-md-preview (GitHub)](https://github.com/bwyan/fcc-md-preview)

### Day 28: February 1, 2017

**Today's Progress**: I worked on the CSS (with Sass) for my Markdown Previewer project:

- [x] Create example.md for testing.
- [x] Add stacked layout for smaller screens.
- [x] Improve typography and fonts.

**Thoughts:** I should be able to finish tweaking the styles tomorrow and call it done.

**Todo:** 

- [ ] Finish the CSS for all of the html elements that markdown supports.

**Link to work:** [bwyan/fcc-md-preview (GitHub)](https://github.com/bwyan/fcc-md-preview)

### Day 29: February 2, 2017

**Today's Progress**: I finished my Markdown Previewer project:

- [x] Finish the CSS for all of the html elements that markdown supports.
- [x] Improve layout on smaller screens.
- [x] Improve typography and fonts.
- [x] Add default content to the `textarea`.

**Thoughts:** This was a fun project that gave me a nice intro to Sass and building a responsive layout without a framework.

**Todo:** Deploy my Markdown project to GitHub Pages and then start scaffolding my next project.

**Link to work:** [bwyan/fcc-md-preview (GitHub)](https://github.com/bwyan/fcc-md-preview)

### Day 30: February 3, 2017

**Today's Progress**: I posted my markdown previewer to GitHub pages and set up the environment for my Camper Leaderboard.

**Thoughts:** Everything went smoothly and I can't wait to start on the project tomorrow.

**Todo:** Start building the components for my next project and connect to the FCC APIs I need.

**Link to work:** [Markdown Preview (GitHub Pages)](https://bwyan.github.io/fcc-md-preview)

### Day 31: February 4, 2017

**Today's Progress**: My leaderboard is functionally complete.

**Thoughts:** This was a pretty simple project and I'm happy with how much I remembered from my other react project and tutorials.

**Todo:**

- [ ] Improve accessibility on the toggle.
- [ ] Improve the styling based on some of the beautiful leaderboard inspirations I found on pinterest.
- [ ] Turn the camper row into its own component (mostly just for a hypothetical case of reusing the same display in other places).
- [ ] Set a fixed size for the table so that it doesn't flash when changing data.
- [ ] Cache or otherwise store the results of each query to minimize requests and delays in toggling results.

**Link to work:** [Camper Leaderboard](https://github.com/bwyan/fcc-leaderboard)

### Day 32: February 5, 2017

**Today's Progress**: Continued work on my leaderboard project.

- [x] Improve accessibility on the toggle.
- [x] Improve the styling based on some of the beautiful leaderboard inspirations I found on pinterest.

**Thoughts:** Just tweaking the css at this point, which is fun but could last forever. 

**Todo:**

- [ ]	Pin the toggle to the top of the screen when scrolling.
- [ ] Improve the styling based on some of the beautiful leaderboard inspirations I found on pinterest.
- [ ] Set a fixed size for the table so that it doesn't flash when changing data.
- [ ] Cache or otherwise store the results of each query to minimize requests and delays in toggling results.
- [ ] Turn the camper row into its own component (mostly just for a hypothetical case of reusing the same display in other places).

**Link to work:** [Camper Leaderboard](https://github.com/bwyan/fcc-leaderboard)

### Day 33: February 6, 2017

**Today's Progress**: Continued work on my leaderboard project.

- [x]	Pin the toggle to the top of the screen when scrolling (Works in Safari and FF. Graceful Degradation ftw.)
- [x] Set a fixed size for the table so that it doesn't flash when changing data.

**Thoughts:** I'm stuck with a table that's just a bit wider than my 320px min-width because the names aren't truncating. It's very tempting to move away from a table even though it's symantically correct.

**Todo:**

- [ ] Improve the styling based on some of the beautiful leaderboard inspirations I found on pinterest.
- [ ] Cache or otherwise store the results of each query to minimize requests and delays in toggling results.
- [ ] Turn the camper row into its own component (mostly just for a hypothetical case of reusing the same display in other places).

**Link to work:** [Camper Leaderboard](https://github.com/bwyan/fcc-leaderboard)

### Day 34: February 7, 2017

**Today's Progress**: Continued tweaking the styling on my leaderboard project, fixed an issue with table sizing, and added new styling for wider screens.

**Thoughts:** The problem with the sizing turned out to be that I was using `<col></col>` instead of `<col />`. Once I did that, everything worked just fine.

**Todo:**

- [ ] Improve the styling based on some of the beautiful leaderboard inspirations I found on pinterest.
- [ ] Cache or otherwise store the results of each query to minimize requests and delays in toggling results.
- [ ] Turn the camper row into its own component (mostly just for a hypothetical case of reusing the same display in other places).

**Link to work:** [Camper Leaderboard](https://github.com/bwyan/fcc-leaderboard)

### Day 35: February 9, 2017

**Today's Progress**: Finished my Leaderboard (except for caching and refactoring) and set up / started scaffolding my recipe app.

**Thoughts:** The problem with the sizing turned out to be that I was using `<col></col>` instead of `<col />`. Once I did that, everything worked just fine.

**Todo:**



**Link to work:** [Camper Leaderboard](https://bwyan.github.com/fcc-leaderboard)

### Day 36: February 10, 2017

**Today's Progress**: Created the Editor and RecipeList components for my Recipe Box app.

**Thoughts:** I was pretty successful but didn't have much time.

**Todo:**
- [ ] Build the Editor form and hook it up so it updates the App's state.
- [ ] Pass the state into the Recipe List and display a list of recipes.

**Link to work:** [Recipe Box](https://github.com/bwyan/fcc-recipe)

### Day 37: February 11, 2017

**Today's Progress**: Finished the items I set it yesterday's Todo.

- [x] Build the Editor form and hook it up so it updates the App's state.
- [x] Pass the state into the Recipe List and display a list of recipes.

**Thoughts:** I'm not happy with how long it took me. I'm relying too much on looking at my previous React projects for reference, rather than relying on my knowledge. I need to be able to apply my knowledge to new contexts (like this project). I'm specifically struggling with how to set unique keys for items in an array when iterating over an array and into DOM elements.

**Todo:**
- [ ] Set unique keys for each element.
- [ ] Figure out how I want to present my recipe details before building any more components or behaviors.

**Link to work:** [Recipe Box](https://github.com/bwyan/fcc-recipe)

### Day 38: February 12, 2017

**Today's Progress**:I decided to use a sidebar/viewer pattern for the UI, so that helped make up my mind on how to build the components. I built the components I needed and hooked them up to set a global "CurrentRecipe" state.

**Thoughts:** I'm still not happy with how much trial and error I'm using, but I *am* happy with how I'm able to quickly solve problem that aren't react-specific, such as what to do if a component is expecting data and doesn't receive it.

I would like to get more fluent in React so that my code is elegant and throws fewer errors when I first write it. I'd also like to start working more with functional stateless components.

**Todo:**
- [ ] Enhance the editor so it can create a new recipe or edit an existing one.
- [ ] In the RecipeViewer, set a unique key for each ingredient in the list.

**Link to work:** [Recipe Box](https://github.com/bwyan/fcc-recipe)

### Day 39: February 13, 2017

**Today's Progress**: I changed App so that it only shows the editor when it's called for, and got the editor to call up an existing recipe. 

**Thoughts:** I'm getting a *little* faster at adding and changing components accurately, but it still requires more thinking than working with JS or jQuery, where I find the answer is more often at my fingertips.

**Todo:**
- [ ] Enhance the editor so it can create a new recipe or edit an existing one.
- [ ] In the RecipeViewer, set a unique key for each ingredient in the list.

**Link to work:** [Recipe Box](https://github.com/bwyan/fcc-recipe)

### Day 40: February 15, 2017

**Today's Progress**: Slowly working through the features in my app.

- [x] Enhance the editor so it can create a new recipe or edit an existing one.

**Thoughts:** I tried a way of handling the editor that involved the App holding a lot more state (and having to pass it to the editor). The one advantage was that I could then show a recipe while creating a new recipe. I decided to simplify because it didn't seem like the extra functionality was worth the complexity. If I did need to create that feature, I'd want to find a different way of coding it.

**Todo:**
- [ ] Save the App's state in LocalStorage.
- [ ] Work on styling.

**Link to work:** [Recipe Box](https://github.com/bwyan/fcc-recipe)

### Day 41: February 16, 2017

**Today's Progress**: Slowly working through the features in my app.

- [x] In the RecipeViewer, set a unique key for each ingredient in the list when displaying the ingredients.
- [x] Refactored a couple of if statements as ternary operators to clean up App's render return.
- [x] Save the App's state in LocalStorage.

**Thoughts:** I tried a way of handling the editor that involved the App holding a lot more state (and having to pass it to the editor). The one advantage was that I could then show a recipe while creating a new recipe. I decided to simplify because it didn't seem like the extra functionality was worth the complexity. If I did need to create that feature, I'd want to find a different way of coding it.

**Todo:**
- [ ] Enable recipe deletion.
- [ ] If recipe is open with ingredients, clicking New Recipe should clear the form inputs.
- [ ] Work on styling.

**Link to work:** [Recipe Box](https://github.com/bwyan/fcc-recipe)

### Day 42: February 17, 2017

**Today's Progress**: 
- [x] Enable recipe deletion.

**Thoughts:** I got stuck with an infinite loop caused by not setting up the button handler correctly. I needed to use `onClick={() => this.deleteRecipe}` but I left out the arrow function, which caused the button to fire immediately and repeatedly on page load. That took most of my hour to debug, but once I found it, the rest was easy.

**Todo:**
- [ ] If recipe is open with ingredients, clicking New Recipe should clear the form inputs.
- [ ] Work on styling.

**Link to work:** [Recipe Box](https://github.com/bwyan/fcc-recipe)

### Day 43: February 18, 2017

**Today's Progress**: 
- [x] If recipe is open with ingredients, clicking New Recipe should clear the form inputs.
- [x] Set editor and viewer so that only one or the other are ever displayed.
- [x] Set default recipes to avoid a totally empty state for new users.
- [x] Started work on the first stages of the layout.

**Thoughts:** I got a lot done today. It feels good to make meaningful progress and not break things.

**Todo:**
- [ ] Work on styling.

**Link to work:** [Recipe Box (Repo)](https://github.com/bwyan/fcc-recipe). [Recipe Box (demo)](https://bwyan.github.io/fcc-recipe).

### Day 44: February 19, 2017

**Today's Progress**: I worked on the UI behavior and styling.

- [x] Make the sidebar slide out of view with a toggle, and when clicking "new recipe".
- [x] Work on mobile layout.
- [x] Minor adjustments to component styling.

**Thoughts:** I got a lot done again today, and I'm also seeing the benefit of breaking nearly every element into components. Even though it might seem unnecessary in a smaller project, it makes reuse easier later on.

**Todo:**
- [ ] Hide the sidebar automatically when selecting a recipe.
- [ ] Keep sidebar in view at all times on larger screens.
- [ ] Continue styling improvements.

**Link to work:** [Recipe Box (Repo)](https://github.com/bwyan/fcc-recipe). [Recipe Box (demo)](https://bwyan.github.io/fcc-recipe).

### Day 45: February 20, 2017

**Today's Progress**: I worked on the UI behavior and styling.
- [x] Hide the sidebar automatically when selecting a recipe.
- [x] Show sidebar automatically when you'd otherwise get an empty content view (like if clicking Cancel while making a new recipe)
- [x] Keep sidebar in view at all times on larger screens.
- [x] Made a few minor improvements to the layout.

**Thoughts:** I need to spend some time learning modern CSS layout techniques. I spent a lot of time wrestling with Flexbox but ended up with very little to show for it. However, I'm happy with how many UI behavior improvements I was able to implement with React.

**Todo:**
- [ ] Continue styling and layout improvements.

**Link to work:** [Recipe Box (Repo)](https://github.com/bwyan/fcc-recipe). [Recipe Box (demo)](https://bwyan.github.io/fcc-recipe).

### Day 46: February 21, 2017

**Today's Progress**: I continued work on the UI behavior and styling.
- [x] When the sidebar is showing on small screens, dim the background and make it hide the sidebar if tapped.
- [x] Minor layout changes.

**Thoughts:** I keep thinking it'd be easier to use a UI framework that already has elements like my sidebar, but this is so much more and rewarding. I wrote my first functional stateless component as well, which is so nice and clean!

**Todo:**
- [ ] Continue styling and layout improvements.
- [ ] Make the content area scrollable.
- [ ] Add `visibility` to the DimmerLayer to improve accessibility, and make the transition animate.

**Link to work:** [Recipe Box (Repo)](https://github.com/bwyan/fcc-recipe). [Recipe Box (demo)](https://bwyan.github.io/fcc-recipe).

### Day 47: February 22, 2017

**Today's Progress**: Short day because I got a late start. Just a couple minor improvements:

- [x] Add `visibility` to the DimmerLayer to improve accessibility, and make the transition animate.
- [x] Fixed a bug preventing the `dimmer-layer` from filling the full width of the screen.

**Thoughts:** I keep thinking it'd be easier to use a UI framework that already has elements like my sidebar, but this is so much more and rewarding. I wrote my first functional stateless component as well, which is so nice and clean!

**Todo:**
- [ ] Continue styling and layout improvements.
- [ ] Make the content area scrollable.

**Link to work:** [Recipe Box (Repo)](https://github.com/bwyan/fcc-recipe). [Recipe Box (demo)](https://bwyan.github.io/fcc-recipe).

### Day 48: February 24, 2017

**Today's Progress**: I got the sidebar scrolling working well, and did a few minor styling tweaks (button sizes, margins, etc.)

**Thoughts:** I've wrestled with a lot of different techniques for making fixed-height elements with scrollable content, but finally found one that works consistently. I also got my iPhone to connect to localhost, which makes testing way easier. If I only knew it was as easy as connecting to my computer's IP:3000.

**Todo:**
- [ ] Fix the landscape scrolling behavior (probably by setting the sidebar to `position: fixed` but making sure it's still visible).
- [ ] Continue styling and layout improvements.
- [ ] Make the content area scrollable.

**Link to work:** [Recipe Box (Repo)](https://github.com/bwyan/fcc-recipe). [Recipe Box (demo)](https://bwyan.github.io/fcc-recipe).

### Day 49: February 26, 2017

**Today's Progress**: Spent the hour working on a fix for…

- [x] Fix the landscape scrolling behavior (probably by setting the sidebar to `position: fixed` but making sure it's still visible).

**Thoughts:** On iPhone 7+ in landscape, the sidebar is too tall, but in the responsive design tool in Safari, it looks correct. I'll need to 

**Todo:**
- [ ] Continue styling and layout improvements.
- [ ] Make the content area scrollable.

**Link to work:** [Recipe Box (Repo)](https://github.com/bwyan/fcc-recipe). [Recipe Box (demo)](https://bwyan.github.io/fcc-recipe).

### Day 50: February 28, 2017

**Today's Progress**: Finished my recipe box!

- [x] Added more recipes 
- [x] Finished enough styling tweaks to feel happy with the app overall.

**Thoughts:** Yesterday I mentioned that on iPhones in landscape, the sidebar is too tall, but in the responsive design tool in Safari, it looks correct. I figured out that it's due to how Safari handles showing and hiding the toolbar. If I give the content a good flick, the toolbar goes away and the page looks correct. 

Overall this was a really fun project and it's cool to see how far it's come from when I was first building form components and wondering how they'd all fit together. I spent more time on it than I planned, but that's mainly because I was having fun figuring out how to build a native-style app in a web browser.

Starting tomorrow, I'm going to re-evalute my 100daysofcode schedule because I expect a strenuous work and home life for the next two weeks. May need to take 2 nights/week to rest and recover.  

**Link to work:** [Recipe Box (Repo)](https://github.com/bwyan/fcc-recipe). [Recipe Box (demo)](https://bwyan.github.io/fcc-recipe).

### Day 51: March 8, 2017

**Today's Progress**: Started Conway's Game of Life

- [x] Set up new react project.
- [x] Scaffolded Grid, Row, and Cell components.
- [x] Studied the rules of the game.

**Thoughts:** This was my first time writing JavaScript in about 2 weeks and first time writing any code in 8 days. I took a much-needed week off, and I'm happy to be back to coding daily (that's the plan!) again.

This particular project feels a lot more Computer-sciency than the last few, and I'm looking forward to the challenge.

Finally, I found a github project for doing Pixel Grids in React, but I've decided to try building my own and see how that goes first.

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 52: March 9, 2017

**Today's Progress**: Worked on Conway's Game of Life

- [x] Make grid adjust it's layout based on the row and column values held in the App's state.
- [x] Determine a data store for the board's alive cells. (I'm using an array of arrays)
- [x] Passed alive cells state into the Grid and Row components.

**Thoughts:** Everything was going great and I didn't need to reference any material to get this working. But I bumped into an issue that stumped me: I can't seem to use indexOf within my component. It works in the console with React dev tools, but I'm getting an error when I try putting it in my code. This is blocking my progress so it's the number one thing I need to do unless I can think of a workaround. (I don't want to store every cell's alive state in an object—it just feels too heavy.)

**Todo:**

- [ ] Figure out how to work with `indexOf` on props.
- [ ] Build a function to toggle the "alive" state of a cell (will require setting up proper refs on the cells)

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 52: March 9, 2017 UPDATE

**Today's Progress**: I just couldn't resist, and kept poking around after I comitted my log. The issue is that I didn't have enough empty arrays to match the number of rows, so the "undefined" error was due to the array address returning undefined. Tonight's easy fix was to create fewer rows, but I'll need a function that keeps the right number of arrays in `aliveCells`.

**Todo:**

- [ ] Build a function to update the `is alive` state to match the number of rows (and remove column values greater than the current number of columns).
- [ ] Build a function to toggle the "alive" state of a cell (will require setting up proper refs on the cells).

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 53: March 10, 2017

**Today's Progress**: 

- [x] Built a function `setGridDimensions` that updates the `is alive` state to match the number of rows (and remove column values greater than the current number of columns).

**Todo:**

- [ ] Build a function to toggle the "alive" state of a cell (will require setting up proper refs on the cells so that they know how to report their own coordinates).

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 54: March 11, 2017

**Today's Progress**: 
- [x] Build a function to toggle the "alive" state of a cell (will require setting up proper refs on the cells so that they know how to report their own coordinates).

**Thoughts:** Wow. That was a really fun coding session. Everything was flowing, my code wasn't generating errors, and I hardly had to look anything up. I really feel like I'm starting to get it now. Javacript continues to feel easier and my brain understands how to get most of the common tasks done in React without much thinkng. I think I spent more time scratching out the "algorithm" than I did connecting everything in React.

**Todo**:

-[ ] Build the algorithm that plays one turn of the game.
-[ ] Get it to repeat indefinitely (try `while gameIsRunning === true` or recursion with `componentDidUpdate`).
-[ ] Build the rest of the UI components (board size, start/stop button, etc.)
-[ ] Ignore click events while the game is playing.


**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 55: March 12, 2017

**Today's Progress**: 
-[x] Scaffold the algorithm that plays one turn of the game.

**Thoughts:** I didn't have much time today but managed to write most of the method. It's not quite working yet, but I think it's due to a helper method `isAlive`. Tomorrow I'll add some `console.log` statements and that'll make it easy to track down the broken point(s).

**Todo**:

-[ ] Build the algorithm that plays one turn of the game.
-[ ] Get it to repeat indefinitely (try `while gameIsRunning === true` or recursion with `componentDidUpdate`).
-[ ] Build the rest of the UI components (board size, start/stop button, etc.)
-[ ] Ignore click events while the game is playing.


**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 56: March 14, 2017

**Today's Progress**: 
I nearly finished one of the most important methods, `setCellToNextStageOfLife`, however I need to have it update all the cells at once instead of updating as it iterates over the loop (which changes the results).

I also started the most important method, `setGameToNextStageOfLife`. It works, but it's dependent on the changes I mentioned above.

**Thoughts:** This took a little longer than I thought, partly because I got interrupted, and partly because I was placing some of my nested if statements in the wrong levels. Between debugging and remembering where I left off, it added up to more time spent than I hoped. I think I have a clear path to finish the methods tomorrow though.

**Todo**:

-[ ] Finish the algorithm that plays one turn of the game. Ensure that it updates state for all cells at the same time.
-[ ] Get it to repeat indefinitely (try `while gameIsRunning === true` or recursion with `componentDidUpdate`).
-[ ] Build the rest of the UI components (board size controls, start/stop/clear buttons)
-[ ] Refactor to improve efficiency.
-[ ] General cleanup (remove TODOs, console.log() statements, or commented out code)

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 57: March 15, 2017

**Today's Progress**: 
-[x] Finished `setCellToNextStageOfLife`and `setGameToNextStageOfLife`. 
-[x] Added (non working) Start/Stop/Clear buttons.

**Thoughts:** Both of the methods are working well, but my algorithm needs some optimization. Right now it takes nearly a second to play one turn on a 20x30 grid.

**Todo**:

THE BEST APPROACH MIGHT BE CREATING MORE IF STATEMENTS THAT ULTIMATELY REDUCE THE NUMBER OF 'NEIGHBORS' THAT HAVE TO BE CHECKED FOR EACH CELL.

-[ ] Optimize the algorithm that plays one turn of the game.
-[ ] Get it to repeat indefinitely (try `while gameIsRunning === true` or recursion with `componentDidUpdate`).
-[ ] Hook up the UI components (board size controls, start/stop/clear buttons) to state.
-[ ] General cleanup (remove TODOs, console.log() statements, or commented out code)

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).


### Day 58: March 16, 2017

**Today's Progress**: I worked on optimizing my algorithm:

-[x] Fixed a bug that was causing the dead cells to evaluate incorrectly.
-[x] Create a default state so I can test the changes under the same conditions each time.
-[x] Refactored my approach to determining which cells are neighbors, by only generating neighbors as needed for testing, rather than generating all 8 neighbors each time. For example, if a dead cell has four alive neighbors, it won't come to life, so we don't need to get neighbor coordinates for neighbors 5 to 8.
-[x] Reordered some conditionals and added `break`s to remove unnecessary loop iterations.
-[x] Found a several more optimizations to implement tomorrow (see below).

**Thoughts:** Some of my work was trial-and-error, but looking through the code and thinking about all the steps required, I was able to find several ways to simplify. I'd love to learn a methodical approach to optimization, but this was a good start.

**Todo**:
#### Optimizations
-[ ] Move from if else to switch statements where possible.
-[ ] Set rules for corner and edge cells and test cells against those first.
-[ ] Refactor the algo to use `makeAlive` and `makeDead` methods instead of `toggleIsAliveState` (because we already know whether the cell will need to be made alive or dead, it's wasteful to check that again).
-[ ] Think: are there other cases where we already know the outcome with certainty after only evaluating some of the neighbors?

#### Overall
-[ ] Optimize the algorithm that plays one turn of the game.
-[ ] Get it to repeat indefinitely (try `while gameIsRunning === true` or recursion with `componentDidUpdate`).
-[ ] Hook up the UI components (board size controls, start/stop/clear buttons) to state.
-[ ] General cleanup (remove TODOs, console.log() statements, or commented out code)

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 59: March 17, 2017

**Today's Progress**: I worked on optimizing my algorithm:

-[x] Move from if else to switch statements where possible.
-[x] Refactor the to use `addToCellsToMakeAlive` and `addToCellsToMakeDead` methods instead of `toggleIsAliveState`, and remove extra `setState`s.
-[x] Hook up a "next" button to step through generations.

Which means I can check this one off:
-[x] Optimize the algorithm that plays one turn of the game.

**Thoughts:** 


**Todo**:
#### Overall

-[ ] Get the game to repeat indefinitely (try `while gameIsRunning === true` or recursion with `componentDidUpdate`).
-[ ] Hook up the UI components (board size controls, start/stop/clear buttons) to state.
-[ ] General cleanup (remove TODOs, console.log() statements, or commented out code)

#### Other performance tweaks if needed/desired

-[ ] Set rules for corner and edge cells and test cells against those first.
-[ ] Think: are there other cases where we already know the outcome with certainty after only evaluating some of the neighbors?

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 60: March 18, 2017

**Today's Progress**: I hooked up the controls, and sorta got the looping to work:

-[x] Get the game to repeat indefinitely (try `while gameIsRunning === true` or recursion with `componentDidUpdate`).
-[x] Hook up the start/stop and clear buttons.

**Thoughts:** 
I can click my "next" button to advance the board in about 24ms. However, with `setInterval` it's taking over 450ms, no matter what values I pass in. I'll need to figure out another way to let the game run indefinitely. Recursion won't work becuase of the number of method instances it would create.

**Todo**:
#### Overall

-[ ] Improve the speed that the game can run at.
-[ ] Hook up the board size fields to state.
-[ ] General cleanup (remove TODOs, console.log() statements, or commented out code)

#### Other performance tweaks if needed/desired

-[ ] Set rules for corner and edge cells and test cells against those first.
-[ ] Think: are there other cases where we already know the outcome with certainty after only evaluating some of the neighbors?

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 61: March 20, 2017

**Today's Progress**: 
-[x] Improve the speed that the game can run at (reliably down to ~80ms per generation).
-[x] Add Generation counter.

**Thoughts:** 
The solution I came up with for speeding up the game is both ingenious and totally insufficient: rather than call the "next generation" function directly, I simulate a click of the "next generation" button (which calls the same function). I have no idea why this works, but it must have something to do with calling the function/having to bind it properly with `const self = this`. I'll need to investigate further, but for now, this hackey fix will allow me to continue to the other aspects of the game.

**Todo**:

-[ ] Hook up the board size fields to state.
-[ ] General cleanup (remove TODOs, console.log() statements, or commented out code)
-[ ] Light styling (I'm not going to go crazy with this one).

**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 62: March 21, 2017

**Today's Progress**: 
-[x] Hook up the board size fields to state.
-[x] Add react-debounce to board size fields to prevent unnecessary data clearing.
-[x] General cleanup (remove TODOs, console.log() statements, or commented out code)

**Thoughts:** 
It was nice to move away from the heavier lifting and do some easier tasks today. That's a good reminder to myself that if I'm feeling overwhelmed or unmotivated, or want a break, it might be a good time to put the bigger things on hold (when I can) and do some cleanup and simpler tasks.

**Todo**:
-[ ] When I first arrive at the board, it will randomly generate a board and start playing.
-[ ] Light styling (I'm not going to go crazy with styling this project).
-[ ] More General cleanup (mainly remove commented out code or unused methods).
-[ ] Do I need to enable wrap-around handling for edges?


**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 63: March 22, 2017

**Today's Progress**: 
-[x] When I first arrive at the board, it will randomly generate a board and start playing.
-[x] Basic visual tweaks.

**Thoughts:** 
It was nice to move away from the heavier lifting and do some easier tasks today. That's a good reminder to myself that if I'm feeling overwhelmed or unmotivated, or want a break, it might be a good time to put the bigger things on hold (when I can) and do some cleanup and simpler tasks.

**Todo**:
-[ ] Light styling (I'm not going to go crazy with styling this project).
-[ ] More General cleanup (mainly remove commented out code or unused methods).
-[ ] Do I need to enable wrap-around handling for edges?


**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life).

### Day 64: March 24, 2017

**Today's Progress**: 
-[x] Add limits on the number of rows and columns that can be used.
-[x] Add error message when number rows or columns is exceeded.
-[x] Add start/stop button states.
-[x] Light styling and layout changes.
-[x] General cleanup (I left some commented out code in the project because I'm hoping some day a React expert can explain why certain things were behaving oddly).

**Thoughts:** 
I'm done! I double-checked that I did all the user stories, and I did. What a great feeling! This one definitely challenged me but it never felt too hard. I enjoyed working on the more CS-based parts of it, like the algorithm, but also liked the feeling of implementing most of my ideas "The React Way" without having to think too hard about it or "translate" my idea from the way I would have done it in jQuery.

One other tidbit: I finally encountered a case where it made more sense to store state in a child component than in the root component. (My GameControls form has an error message that can be shown/hidden.)

**Todo**:
-[ ] Start the next project.


**Link to work:** [Conway's Game Of Life (Repo)](https://github.com/bwyan/fcc-life). [Conway's Game Of Life (demo)](https://bwyan.github.io/fcc-life).

### Day 65: March 25, 2017

**Today's Progress**: 
-[x] Set up environment and repo for my Roguelike Dungeon Crawler.
-[x] Planned a model for my state and some other aspects of the project.

**Thoughts:** 
It's always fun but a little intimidating to start a new project. I'm looking forward to it though!

**Todo**:
-[ ] Start scaffolding the components, and reuse what I can from the `Grid`, `Row`, and `Cell` components in my Game of Life.
-[ ] Build a level

**Link to work:** [Into the Dungeon (Repo)](https://github.com/bwyan/fcc-life).

### Day 66: March 26, 2017

**Today's Progress**: 
-[x] Learned about tilemaps and decided on a data structure. Built a simple map object.
-[x] Built a basic character object.

**Thoughts:** 
So far, this isn't so bad. The reading I did about tile maps (once I learned what they were called) confirmed my hunch that I should use a simple array or array of arrays. I'm starting out with an array of arrays so that I can re-use some of my code from the Game of Life project.

As I started writing the code today, I could sense my brain getting primed to figure out the details. At the moment, it feels like my biggest bottleneck will be typing the code—not wrestling with how to implement it. Let's see if that optimism carries through the whole project!

**Todo**:
-[ ] Start scaffolding the components, and reuse what I can from the `Grid`, `Row`, and `Cell` components in my Game of Life.
-[ ] Build a 'real' level (and possibly a level editor if I want more than a couple small levels!).

**Link to work:** [Into the Dungeon (Repo)](https://github.com/bwyan/fcc-life).

### Day 67: March 27, 2017

**Today's Progress**: I did a lot of scaffolding:

-[x] Create `data/weapons.js` with a Weapon constructor and a weapons object.
-[x] Create maps.js to store level map data.
-[x] Create playerLevels to store stats (max health, attack, etc.) for each experience level.
-[x] Bring in the Grid, Row, and Cell (now Board, Row, and Tile) components from my Game of Life project.

**Thoughts:** 
My comment about my bottleneck being the typing is totally true so far. That could change, but for now it's a blast to type furiously to get all the ideas out as quick as possible. The scope and scale of this project—in terms of the amount of data and components I'll need—prompted me to get more organized in how I store my code. With the game of life, I didn't mind keeping it all in one place, but even by the end of that project, it was getting tough to manage. For this project, I'm forcing myself to be disciplined with code organization, even though at first it feels like it's slowing me down a little.

**Todo**:
-[ ] Build what I need to get a simple level to appear.
-[ ] Build the HUD to show player stats and game info.
-[ ] Build the methods needed to move around the board and get stopped by walls.
-[ ] Build the methods needed to pick up weapons and health.
-[ ] Build an enemies.js file to store enemy names and stats.
-[ ] Build the methods needed to fight enemies.
-[ ] Build the methods needed to "exit" a level and go to the next one.
-[ ] Build a level editor.
-[ ] Build some 'real' levels.
-[ ] Helper UI for various states: game over, winning, etc.

**Link to work:** [Into the Dungeon (Repo)](https://github.com/bwyan/fcc-life).

### Day 68: March 28, 2017

**Today's Progress**: I did a lot of scaffolding:
-[x] Build everything I need to get a simple level to appear.
-[x] Build the methods needed to move around the board and get stopped by walls.

**Thoughts:**
This continues to be an easy project in terms of the algorithms and methods needed, and yet I'm learning a lot from it. As with yesterday, I'm thinking a lot about how to organize my code including where to put each piece, what to name my variables and methods, how to structure the data in my data files, how to keep functions relatively small, etc.

There's definitely a balance to strike between overbuilding and building for the future, I'm sure I'll need to refactor various pieces during the process, but so far it's working well and most of the code feels pretty clean. One thing I'd like to explore is moving some of my App's methods into a separate file, just so it doesn't get too long. Before I do, I want to read up on the best practices for doing so.

I'm most proud that I found a use for Classes in my tiles and weapons files, which saves a lot of typing and allows me to add new features to the objects as the game grows. 

**Todo**:
-[ ] Hook up keyboard event listeners to control player movement.
-[ ] Build the HUD to show player stats and game info.
-[ ] Build the methods needed to pick up weapons and health.
-[ ] Build an enemies.js file to store enemy names and stats.
-[ ] Build the methods needed to fight enemies.
-[ ] Build the methods needed to "exit" a level and go to the next one.
-[ ] Build a level editor.
-[ ] Build some 'real' levels.
-[ ] Helper UI for various states: game over, winning, etc.

**Link to work:** [Into the Dungeon (Repo)](https://github.com/bwyan/fcc-life).

### Day 69: March 29, 2017

**Today's Progress**: Refactor Party!
-[x] Refactored every function that interacts with the map, so my tilemaps can use flat arrays instead of nested arrays.
-[x] Added getTile and getTileIndex methods to enable flat arrays.
-[x] Refactored a few methods to improve readability.

**Thoughts:**
A trusted engineer at work suggested that I refactor my game to use flat arrays for my tilemaps instead of nested arrays. I thought it would make for more complex-looking code (always having to derive the tile coordinates from an index, or vice-versa). However, he pointed out that once you have the functions, getTile and getTileIndex, the code is more readable and also easier to maintain in the long run.

I decided to go for it before the project got any larger. It was a fun exercise to keep making changes and tracking down all the console errors I was getting, until finally everything worked again. Even though I don't have any new features today, I'm glad for both the sake of my education and the sake of the project that I spent tonight refactoring.

**Todo**:
-[ ] Hook up keyboard event listeners to control player movement.
-[ ] Build the HUD to show player stats and game info.
-[ ] Build the methods needed to pick up weapons and health.
-[ ] Build an enemies.js file to store enemy names and stats.
-[ ] Build the methods needed to fight enemies.
-[ ] Build the methods needed to "exit" a level and go to the next one.
-[ ] Build a level editor.
-[ ] Build some 'real' levels.
-[ ] Helper UI for various states: game over, winning, etc.

**Link to work:** [Into the Dungeon (Repo)](https://github.com/bwyan/fcc-life).

### Day 70: March 29, 2017

**Today's Progress**:
-[x] Hook up keyboard event listeners to control player movement.(Arrow keys and WASD.)
-[x] Split 'handleMove' into three methods: `handleKeyDown`, `nextPlayerCoordinates`, and `handleMove`.
-[x] Build the HUD to show player stats and game info.

**Thoughts:**
A little refactoring? Key bindings? Some new components? This is a really productive night!

**Todo**:
-[ ] Build the methods needed to pick up weapons and health.
-[ ] Build an enemies.js file to store enemy names and stats.
-[ ] Build the methods needed to fight enemies.
-[ ] Build the methods needed to "exit" a level and go to the next one.
-[ ] Build a level editor.
-[ ] Build some 'real' levels.
-[ ] Helper UI for various states: game over, winning, etc.

**Link to work:** [Into the Dungeon (Repo)](https://github.com/bwyan/fcc-life).

### Day 71: March 29, 2017

**Today's Progress**:
-[x] Add an Item class that can provide multiple rewards.
-[x] Build `changeWeapon()` to let the player pick up new weapons.
-[x] Build `pickUpItem()` to pick up an item and earn it's rewards.

**Thoughts:**
This was a little tougher than I thought because it exposed some flaws in my architecture (they're fixed now). I also got stuck when I realized I can't add weapons to the board (the weapons file is separate from the rest of the tiles, so I need to figure that out).

**Todo**:
-[ ] Refactor to allow me to place weapons on the board (If I move weapons into tiles.js, I'll need to update `changeWeapon()`).
-[ ] `changeWeapon()` should drop the old weapon on the player's tile.
-[ ] `pickUpItem` should accept coordinates as an argument and clear the item listed at the coordinates (if the coords match the item name).
-[ ] Build an enemies.js file to store enemy names and stats.
-[ ] Build the methods needed to fight enemies.
-[ ] Build the methods needed to "exit" a level and go to the next one.
-[ ] Build a level editor.
-[ ] Build some 'real' levels.
-[ ] Helper UI for various states: game over, winning, etc.

**Link to work:** [Into the Dungeon (Repo)](https://github.com/bwyan/fcc-life).