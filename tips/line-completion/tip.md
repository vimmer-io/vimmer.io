You can use `<C-x>` followed by `<C-l>` in insert mode to complete whole lines. This is useful if you know that the line you're currently typing exists in the document already, and you want to duplicate it here without finding and yanking it first.

Furthermore, subsequently typing `<C-x><C-l>` will complete the _following_ lines, so you can keep hitting `<C-x><C-l>` to type in a bunch of lines as if by magic.

**Give it a try in the editor.** Start typing some text that is identical to the start of one of the existing lines at the bottom of the buffer, then keep hitting `<C-x><C-l>`.
