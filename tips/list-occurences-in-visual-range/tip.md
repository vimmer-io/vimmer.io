Yesterday, we saw how we can [search only within a visual range](https://vimmer.io/tip/searching-inside-visual-range). This is _really_ useful —  but sometimes overkill. A lot of the time, you just want to see whether or not an instance of a pattern actually _exists_ within a visual range. Is there an easier way to do that?

Yes! The easiest way to do this that I've found is using the global command, which we [already have a great lesson about here](https://vimmer.io/lesson/the-insane-power-of-vims-global-command). We can use the global command to _list the lines containing a pattern within a range_, which is enough to answer our question of "does this line range contain a match?"

**Try this in the editor** — visually select the interesting line range, then use the global command `:g/foo` to print out all of the instances of `foo` within that range.
