The `".` register keeps track of the last inserted text in Vim. `<C-r>` followed by the name of a register in insert mode puts the contents of that register. Combining these two facts, we know that repeating the last inserted text can be done using `<C-r>.` in insert mode.

**Try it in the editor.** Type your name at the end of the first line, then use this trick to insert your name at the _start_ of the second line.
