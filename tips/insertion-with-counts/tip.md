Most insertion commands — like `i`, `I`, `a`, `A`, `o`, `O`, and so on — accept a count. If you type a count in normal mode _before_ hitting an insertion map, like `10A`, then type your text, the insertion will be repeated that many times.

This means that you can do things like:

- `3Afoo<esc>` to append `foo` to the current line 3 times
- `10ohello world<esc>` to add 10 new lines with the text `hello world`
- `5I--<esc>` to prefix the current line with 5 `-` characters

**Try it in the editor!**
