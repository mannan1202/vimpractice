# Vim daily practice 

## Basic commands
```
:q                          = command to quit with no changes in file
:q!                         = command to force quit with changes in the file
:!                          = the commnad will run in shell for eg !ls -al
:w                          = saves the file
a                           = opens the insert mode post the cursor position
o                           = opens the insert mode on the new line
A                           = opens the insert mode at the end of the line
I                           = opens the insert mode at the start of the line
O                           = opens the insert mode above the current line
u                           = undo steps
Ctrl + r                    = redo steps
v                           = for visual mode, in this mode text is highlighted
d                           = delete the letter (it performs as cut operation as well)
y                           = yanking(copying) the letter
dd                          = deletes the whole line (it performs as cut operation as well)
yy                          = yanking(copy) the whole line
p                           = paste the text after or below
P                           = paste the text before or above
<number>dd                  = deletes the number of lines specified
c                           = changes the letter
cc                          = changes the whole line does not delete the line
D                           = delete the rest of the line from current position of cursor
C                           = changes the rest of the line from current position of cursor
r<replace-character-with>   = replace a single character from normal mode to insert mode directly
w                           = go forward word legal character are space and hyphen -
b                           = go backward word legal character are space and hyphen
db                          = delete a word backward
diw                         = delete the word when the cursor is middle of the world
ciw                         = change inside the word when the cursor is middle of the world
e                           = positions the cursor at the end letter of word
0                           = goes to the start of the line
$                           = goes to the end of the line
d0                          = delete the entire text till start of the line from cursor point
d$                          = delete the entre text till end of the line from cursor point
de                          = delete the text till the end of the word
yiw                         = yanks the inner word for copy and you can paste it using p command
ci"                         = change the inner text between double quotations
di"                         = delete the inner text between double quotations
yi"                         = copy inner text of double quotes and paste it somehwere
%                           = to go back and forth of curly bracket
d%                          = to delete eveything inside the curly bracket
t<character> / f<character> = jumps before the character you are searching / jumps to the character you are searching
dt<character>/df<character> = delete all before the character/ delete everything till the character
T<character> / F<character> = jumps backwards before the charater/ jumps backwards to the character
gg                          = start of the file
G                           = end of the file
<linenumber> G              = go to the line number
```

## Advanced Commands

```
V                          = visual line mode, selects the entire line
Ctrl + v                   = select column wise / can be combined with d,y,r commands
>>                         = indents the text right
<<                         = indents the text left
:/<searchterm>             = search the term in the file
n                          = to search iteratively forward
N                          = to search iteratively backward
#                          = goes backward search the word where the cursor is currently present
*                          = goes forward search the word where cursor is currently present
m<enter-a-character>       = bookmark the a specific code line or function and type '<enter-a-character> to reach there
zz                         = to center in the viewport the current line
:%s/<text>/<replacetext>/g = command to search and replace the text in entire file
:s/<text>/<replacetext>/g  = command to search and reaplce the text in select text using v (visual mode)
.                          = repeates the last command run eg you press dd and press . than it will run dd
```

## Register Mode
```
:reg            = to enter registery mode
"<number>p      = first run :reg, takes the text of the register you want and pastes it at the current cursor position
"+p             = copies from the system clipboard
"0p             = yanked a line and than deleted a line, p pastes delete line content, this command it pastes the yanked line content
qa              = use to start recording macro, <use combining commands> <Esc>
@<macro-letter> = to execute the macro
```


