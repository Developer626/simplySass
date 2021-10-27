# General TODOs
- [ ] Refactor TODO List
- [ ] Move Big TODOs here to clean up some of the code.
- [ ] Get it on NPM? What other platforms can I put it on?
- [ ] Make a Document/Wiki page
- [ ] Create a HowTo for using simplySass?
- [ ] Find out how to make a release
- [ ] Like gridlex (which I think has the code moved into different functions) have media request code moved/made all in one spot.
- [ ] Add more info to the README.md
- [X] (Done, for now) TODO Write a better README.md
- [ ] Update README.md and find out how to add the features that tell it's status and other info at a glance.
- [X] Create a feature list to list out wanted ones
- [ ] Update Feature List
- [X] Rewrite this list as a markdown
- [ ] Is the _standards file nessasary?
- [X] Design and create a Logo for this project.
- [ ] Make a way for the code to output some fallback code (@supports()) when using more newer css code.
- [ ] A minified version of the project.
- [ ] Update FEATURES.md (Add to "Wanted Features" and "Current Featrues")
- [ ] Remove TODO-List.txt



# _color TODOs
- [ ] Make a color checkers to help users know the if text will be visible.
    * Maybe a function that will output two color that is visible that takes in 
     the colors being tested ($background, $text-color), a minimum contrast level
     ($contrast: 50% <-- in percentage) to have between the two colors, and outputs
     a list of colors on either side of the text-color that matches the requirements
- [ ] Make these color functions work in different color spaces
- [ ] Comment and maybe name the color functions to their color spaces that they work in.
- [ ] Make the gradient function take more starting colors to work with. ex. (c1 <-> c2 <-> c3)
- [ ] Make a function that outputs the contrast level, between at least two colors.
- [ ] Write better comments for each function.
- [X] Rewrite the function that choose color harmonies in _colors for the mixins that reside in _mixins. (I broke something. My grammar. LOL)
- [ ] Transfer TODOs, that can be moved, from _color to here.
- [ ] Document _colors partials section


# _flexbox TODOs
- [-] Check if media queries here will merge with the ones in _grid if they have the same attributes. (Ignore this one.)
- [ ] Make a set of mixins for _flexbox
- [ ] Add columns to the _flexbox partials
- [ ] Look up some Flexbox patterns and try to implement them.
    * Flexbox patterns: https://www.youtube.com/watch?v=vQAvjof1oe4 Maybe start here and look for more online to see what people want.
- [ ] Document _flexbox partials


# _functions TODOs
- [ ] Think of some functions that would work here.



# _grid TODOs
- [ ] Future idea, Make the .grid-item* take a chosen name from the user so they have more control?
- [ ] Based on the idea above, have the grid-item do it all. 
    * Have it check for the type `<number>`, `<list>`, and `<map>` then respon accordingly.
- [ ] Add place-items to the _grid/_sub-grid code (replaces justify/align-items?)
- [ ] Add new CSS code to _grid() 
    * place-items, 
    * grid-template? 
    * place-self(? this can be added in the grid-items code itself)
    * align-content(_grid and _sub-grid?), 
    * place-content 
    * grid-auto-(colemns/rows)
    * grid-auto-flow
    * grid (the version like CSS background?)
    * Maybe for the grid-template, I can add it so that it or the other code is used.
- [ ] See if there's a way to make it easier to overlap items.
- [ ] Should I have to manually enter in all the data for tablet and desktop in the _grid function? 
    * If they do, it will allow for cleaner code. but then it will mean that people using the library will have to write more in.
    * What is something that is common that doesn't change often? Maybe that won't need to be changed, so there's a mix of items
        that don't need to be "changed" and some that do. 
        * Ex. The padding on the sides of _grid
- [ ] While _sub-grid() needs to be separate to do it's work, can I combine the grid-items and sub-grid-items into one so
      it will generate less code and hopefully make it easier to work with?
- [ ] Another way to cut some code would be to remove the repeat() from the outputed code when the associating section is equal to 1.
- [ ] Have _grid check to see if $rows and $cols has been sent a string, because this causes them to only output one --grid-item
        being that they only see a length of 1 from each making 1 * 1 = 1.
- [ ] Why does _grid produce code that outputs justify-content instead of having it inside of .grid itself?
- [ ] grid-template-areas works without the need to predefine cols and rows. Add this functionality into _grid()
    * Make --cols and --rows only outputed if values are added to it.
    * CSS variables will need to be tested to accomplish this. Will null or none ruin it for grid-template-areas?
    * https://www.youtube.com/watch?v=CVKbe4RaUZQ&t=264s
- [ ] Add as many features from _sub-grid() to _grid() that will work.
    * Based on some of the ways the methods/functions/features that I want in _grid, they will most likely have to be
      added to _sub-grid(). This is do to the padding that is involved in _grid() which messes up how things fall into
      place. I will still need to test out all of the features I wish to add, it may be possible to add some of them.
- [X] Add an S to the end of grid-item and grid-area
- [ ] Can I make _grid create --grid-items that are --grid-area? Would that be benificial?
- [ ] Make a variable for grid-items that can hold a prefix to name the class, if none then name it grid-item-#
- [ ] Add better documentation to _grid partials
- [ ] See about combining sub-grid and grid mixins to shorten code
- [ ] Try and see if auto-fill and auto-fit will work like I tried before. (_sub-grid?)



# _mixins  TODOs
- [X] This file is broken. It calls functions that have been moved and don't exist anymore. Fix it.
- [ ] Go through each mixin and see what can be removed.
- [ ] For Mixins that are kept, see what can be changed to make them more usefull/robust.
- [ ] Make a button mixin
- [ ] Make a card mixin
- [ ] Make a nav-bar mixin


# _standards TODOs
- [ ] TODO See if this file is really needed.


# _variables TODOs
- [ ] This needs more colors?
- [ ] What other variables is good to put here?


# test.scss TODOs