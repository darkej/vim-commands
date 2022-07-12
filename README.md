## Vim useful commands

Here I collected all the most usefull commands that I use in a daily work.
I will not provide here some basics like `w`, `b`, `e`.


---
`ggdG` - remove all lines in current file

`u` - undo

`R` - reundo

`o` - add new line bellow and go to insert mode

`O` - add new line above and go to insert mode

`A` - go to the end of line and enable insert mode

`P` - paste line above current line

`:reg` - check list of copy register

`"<register_number>p` - paste from given register (ex `"1p"`). Deleting overides current yank but current yank is always at 0 register so you can yank line, go and delete some and then `"0p`.

`/` - find given string (hit enter to find). Navigate founded pattern by `n` and `N`.

`?` - same as above but backwards

`f` - find character in line

`F` - same as above but backwards

`0` - jump to begginig of a line

`0w` - jump to begging of a line word

`$` - jump to end of a line

`*` - will find next occurence of word under cursor

`#` - same as above but backwards

`;` - repeat last command

`==` - indend - based on default seting - line under paragraph

`[]` - jump between paragraphs

`dt<character>` - delte till provided character (ex. `dt"`, `dt<space>`)

`df<character>` - delte till and also provided character (ex. `df"`)

`diw` - delete whole word under cursor

`ciw` - change word under cursor

`r<character>` - repalce character under the curoser to given character

`V; select lines ; S< ; provide html tag` - surround selected line by given html tag

`ysiw<character>` - surround word under cursor by given character (ex `ysiw"`)

`yss<character>` - surround entire line by given character (ex `yss(`)

`ds<character>` - delete surround character (ex `ds"`)

`cs<character><new_character>` - change surround character (ex `cs"'`)

`dst` - delete surrounding tag

`:%s/one/two/g` - find `one` and replace it to `two` in entire file

`:.,5s/one/two/g` - from current line till 5 find `one` and replace it to `two`
