Some Vimmers think that the cursor can sometimes be a bit hard to see. If you agree, Vim has two options that we can use to make the position of the cursor more obvious.

The first is the `cursorline` (`cul`) option. This highlights the line that the cursor is currently on. You can enable this with `:set cursorline` or `:set cul` in Vim.

The second is the `cursorcolumn` (`cuc`) option. This highlights the column that the cursor is currently on. You can enable this with `:set cursorcolumn` or `:set cuc` in Vim.

If you enable _both_, you get a neat 'crosshairs' effect that makes it super clear where your cursor is in the buffer.

**Give it a try in the editor.** First enable `cursorline` with `:set cul`, then enable `cursorcolumn` with `:set cuc`. Then try moving the cursor around — it's much easier to keep track of now!
