In Vim, the `p` key is used for _putting_ (otherwise known as pasting) text from a register. The `p` key leaves the cursor at the _beginning_ of the newly-putted text — `gp`, however, puts the cursor just _after_ the newly-putted text.

At glance, this doesn't seem very useful. But it is a good keymap to know!

Because `gp` places the cursor at the _end_ of the newly-putted text, it behaves differently when it is repeated with the `.` command. This is useful for when you want to insert a particular block of text between a set of lines.

**Give this a go in the editor.** Yank the `return false` line under the _first_ `case` statement in the `switch` with `yy`. Then, put it under the _second_ case statement using `gp`. Then, repeat the same action for the other `case` statements using the `.` keymap in normal mode.
