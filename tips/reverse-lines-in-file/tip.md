To reverse the lines in a file, you can use the follow invocation of Vim's global command:

```
:g/^/m0
```

Now, this is fairly obscure — here's how to read it:

- `:g` is saying 'run the global command'
- `/^/` defines a regular expression that matches _any line_
- `m0` is an Ex command that means 'move the current line to line 1' (the `:m` command moves to one _below_ the targeted line, hence we have to put `0` if we want the line to appear on line `1`)

Altogether, this is saying:

> For each line in the file, move it to line 1

Since the global command works in a top-to-bottom manner, this has the effect of reversing the order of the lines in the file!

**Give it a try in the editor!**

If you want to learn more about the global command, [check out our lesson](https://vimmer.io/lesson/the-insane-power-of-vims-global-command)!
