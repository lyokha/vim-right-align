Vim-right-align
===============

Use command `:RightAlign` to align the current line to the right border,
the optional argument indicates that the position of the cursor must be
kept. Global variable `g:RightAlign_RightBorder` will be used as the position
of the right border: if not set then the value of option `textwidth` will be
used instead. If global variable `g:RightAlign_ShiftRound` is set then the
start position of the line after motion will be shiftwidth-fold, otherwise
the start position will depend on whether option `shiftround` is set.
Default value of `g:RightAlign_ShiftRound` is `1`.

Recommended mappings are

```vim
    imap <silent> <C-b>  <Plug>RightAlign
    nmap <silent> <C-k>b :RightAlign<CR>
    vmap <silent> <C-k>b :RightAlign<CR>
```

