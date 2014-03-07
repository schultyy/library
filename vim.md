# vim-shortcuts

> vim gedoens

## Custom settings per file type

Described here: http://stackoverflow.com/questions/158968/changing-vim-indentation-behavior-by-file-type

## Vertical split size

    :vertical resize <num>
    
## Horizontal split size

    :resize <num>

## Navigate between ctags matches

    :tn[next]
    :tp[revious]
    :ts[elect]
    
## Navigate to previous file

    Ctrl+O
    
## Jump to tag

Position the cursor on symbol and press

    Ctrl+]

## Reset search highlighting

    set hlsearch!

## Select all text

    ggVG
## Convert split modes

To change two vertically split windows to horizonally split

    Ctrl-W t Ctrl-W K

Horizontally to vertically:

    Ctrl-W t Ctrl-W H

Explanations:

`Ctrl-W t` makes the first (topleft) window current `Ctrl-W K` moves the current window to full-width at the very top `Ctrl-W H` moves the current window to full-height at far left


## Multiline comment

First enable block visual mode

    Ctrl+V

Then select rows

    Shift+i

Enter comment char (i.e. `#` or `//`)

Press 

    ESC

It takes a second until the comments appear.


## Selection stuff

[Vim: faster way to select blocks of text in visual mode](http://stackoverflow.com/a/7407095)
> In addition, you can also expand your selection using pattern searches.

> For example, `v/foo` will select from your current position to the next instance of "foo." If you actually wanted to > expand to the next instance of "foo," on line 35, for example, just press `n` to expand selection to the next instance, and so on.
> update

> I don't often do it, but I know that some people use marks extensively to make visual selections. For example, if I'm on line 5 and I want to select to line 35, I might press `ma` to place mark a on line 5, then `:35` to move to line 35. `Shift + v` to enter linewise visual mode, and finally ``a` to select back to mark `a`.
