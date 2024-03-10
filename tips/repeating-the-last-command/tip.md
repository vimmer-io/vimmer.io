You can repeat the last command by typing `@:` in normal mode.

This works because the `":` register contains the last executed command. Combined with the `@` key, which is for running macros, we can read `@:` as running the contents of the `":` register as a macro.

This is particularly useful for repeating commands that you don't have a pre-configured mapping for. For example, I use this all the time when I'm working with the _quickfix list_ — I type `:cnf` to jump to the next file in the list, then type `@:` to jump over the subsequent files.

**Let's try it in the editor.** Use the `:center` command to center one of the lines in the document, then use `@:` in normal mode to center some of the other lines.
