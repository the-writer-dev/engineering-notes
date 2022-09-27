This is the collection of (neo)vim tips that I wish I knew when I started

### Movement
DO not leave the home row! h, j, k, l are your best friend from now on :) <br/>
`h` - left <br/>
`j` - down <br/>
`k` - up <br/>
`l` - right <br/>
`2j` - jump down 2 lines <br/>
`2k` - jump up 2 lines <br/>

`w` - jump to the next word <br/>
`b` - jump back the previous word <br/>

`0` - jump to the very first character in the line <br/>
`$` - jump to the very last characteer in the line <br/>

`i` - insert before cursor <br/>
`a` - insert after cursor <br/>
`I` - insert at the beginning of the line <br/>
`A` - insert at the end of the line </br>

`''` - move cursor to its previous position`

### Modification
Undo and redo <br/>
`u` - undo <br/>
`ctrl+r` - redo <br/>

Deleting lines <br/>
`ggdG` - delete all without copying into the clipboard dd - delete a line <br/>
`{number}dd` - delete next number lines <br/>

Substitute chars and lines <br/>
`s` - substitute a character <br/>
`S` - substitute a line <br/>

Search without case sensitivity
`/\cctx` - find ctx without case sensitivity!

Search and deleting lines <br/>
`:g/<pattern>/d` - delete all lines containing the pattern <br/>

`f` - jump to next occurrence of character <br/>
`F` - jump to the previous occurrence of character <br/>

Search and replace <br/>
:[range]s/{pattern}/{string}/[flags] <br/>
`%s/foo/bar/g` - replace all occurence of foo with bar <br/>
`s/foo/bar` - replace foo with bar in the current line <br/>

Clipboard history <br/>
`:reg` - find the history "1p - paste what's registered at 1 after the cursor <br/>

### Misc <br/>
Jump back to previous cursor <br/>
`ctrl + o` <br/>

Make lines lowercase or uppercase <br/>
With visual mode, select text and u for lowercase U for uppercase <br/>
