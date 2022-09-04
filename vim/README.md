This is the collection of (neo)vim tips that I wish I knew when I started

### Movement
DO not leave the home row! h, j, k, l are your best friend from now on :) <br/>
`h` - left <br/>
`j` - down <br/>
`k` - up <br/>
`l` - right <br/>
`2j` - jump down 2 lines 
`2k` - jump up 2 lines

`w` - jump to the next word <br/>
`b` - jump back the previous word <br/>

`0` - jump to the very first character in the line <br/>
`$` - jump to the very last characteer in the line <br/>

`i` - insert before cursor <br/>
`a` - insert after cursor <br/>
`I` - insert at the beginning of the line <br/>
`A` - insert at the end of the line </br>

### Modification
Undo and redo <br/>
`u` - undo <br/>
`ctrl+r` - redo <br/>

Deleting lines <br/>
`ggdG` - delete all without copying into the clipboard dd - delete a line <br/>
`{number}dd` - delete next number lines <br/>

Substitute chars and lines
s - substitute a character
S - substitute a line

Search and deleting lines
:g/<pattern>/d - delete all lines containing the pattern

f - jump to next occurrence of character F - jump to the previous occurrence of character

Search and replace
:[range]s/{pattern}/{string}/[flags]

%s/foo/bar/g - replace all occurence of foo with bar s/foo/bar - replace foo with bar in the current line

Clipboard history
:reg - find the history "1p - paste what's registered at 1 after the cursor

Misc
jump back to previous cursor
ctrl + o

make lines lowercase or uppercase
With visual mode, select text and u for lowercase U for uppercase
