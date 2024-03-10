You can use the `<C-a>` and `<C-x>` keys to increment and decrement numbers in Vim.

If there's a number under your cursor, `<C-a>` will cause the number to increment and `<C-x>` will cause it to decrement. If there's no number under the cursor, Vim will take you to the nearest number on the line (moving toward the end of the line) and increment/decrement that.

These keymaps also accept a count, so you can type `10<C-a>` in normal mode to increment a number by 10.

This is really useful for fixing off-by-one errors or playing with array indices.

**Try it in the editor.** Use the `<C-a>` and `<C-x>` commands to change the port number on line 6.
