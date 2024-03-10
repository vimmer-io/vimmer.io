The `s` key in normal mode deletes the character under the cursor and immediately enters insert mode. This is one keystroke shorter than `xi`, which does the same thing. But `s` is also repeatable with the `.` operator!

**Let's try it in the editor.** The mathematical expressions are missing spaces between the digits and the operators. E.g. we've got `1+3`, but we really want to write `1 + 3`. Let's use the `s` key to fix these up. Place your cursor on a `+` symbol, then type `s + ` in normal mode. You can then move to any other `+` and hit `.` to repeat!
