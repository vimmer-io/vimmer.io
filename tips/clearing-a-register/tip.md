There are two ways that you can clear a text register in Vim:

- You can use `:let @x = ""` to set the content of `"x` to the empty string
- You can type `qxq` in normal mode

The first one is fairly self-explanatory — we use the `:let` command to explicitly clear out the content of the register.

But what about the second one? Why does `qxq` in normal mode clear the `x` register? Let's walk through it.

- `qx` starts recording a new macro into the `"x` register
- `q` immediately stops recording

So, altogether, `qxq` records _nothing_ into the `"x` register. This has the effect of clearing it out.

**Give it a try in the editor.** Yank the first line into the `"x` register with `"xyy`, then inspect the content of the register with `:reg x`. You should see that the line is in there. Then, try typing `qxq` and again inspect the register with `:reg x`. You should see that it's now empty.
