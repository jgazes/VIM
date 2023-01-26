# Editing Methods in Vim #
## Alter and insert ##
-There are multiple ways aside from pressing 'i' to enter insert mode
	- Shift i inserts text at the start of the line
	- shift a inserts text at the end of the cursor
	- 'o' will add text to a line below, shift 'o' above
	- 's' replaces chracter and enters insert mode
	- 'r' replace character 
	- shift J combines

## Change Case ##
- ~ or shift ~ will change the case of a character
- g shift U changes the case of defined context to uppercase, gu will be lowercase

## Revert and Restore ##
- u is undo to revert and restore
- . is redo
- :earlier <time> will revert the file back to an earlier time
- :later <time> will restore back to a newer time

---

## Deleting Text in Vim ##
In normal mode
- 'x' deletes a single character
- d<value> eg dd deletes an entire line
- d^ will remove everything to the start of the line
- d$ will remove everything to the end of the line
- can pair with any command that indicates movement eg 3dw would be 3 words
- cw will replace word

## Selecting, Copying, and Pasting ##
- v to enter visual mode
- Shift v is a per line visual mode
- Ctrl v is a blockwise visual mode
- o and shift o changes the corner of the block in blockwise visual mode
- gv will reselect previous sections
- u or shift u will change to upper or lowercase
- d will delete everything
- shift > or shift < will tab in or back
- Still in visual mode, to copy we can press y (yank) to copy, p to paste after cursors location

## Searching in Vim ##
- in normal mode, hit / <term> to search for a term
- n or Shift 8 (*) to find the next instance of that search
- shift n or # to find previous
- question mark (?) to search from the bottom
- -\> for whitespace

## Replacing Text in Vim ##
- in normal mode
- : to enter command mode
- s/<term>/<TERM>
- percent % indicates we would like to work with the entire document
- we can add a g to the end to indicate we would like to change all instances of the term, not just the first
- to approve the changes before they happen, we can add a c to the end, then we we will be asked if we want to change
- if we add an i, it will perform a case insensitive search
- gci
- :#,#s/<term>/<TERM>/g to specify line numbers that you would like to search through

## Recording in Vim ##
- Recording actions to perform repetitive macros	
