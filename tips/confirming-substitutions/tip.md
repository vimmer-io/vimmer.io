Sometimes, when you're using the `:substitute` command, you don't want to replace _everything_ that your pattern matches. Sometimes, you want to be able to go through the matches one by one, and confirm whether you want to substitute on a case-by-case basis.

Vim has a flag for the `:substitute` command that allows us to do this.

Let's say you have a substitution to replace all instances of `foo` with `bar` in the buffer. The command for doing something like this is `:%s/foo/bar/g`. To make Vim confirm each match before performing the substitution, you can add the `c` flag to the end of the substitution command — e.g. `:%s/foo/bar/gc`.

This drops us into an interactive mode where we can:

- confirm substitutions with `y`
- skip making substitutions with `n`
- perform _all_ of the remaining substitutions with `a`
- stop making further substitutions with `q`

**Let's try this in the editor.** Try using this trick to replace all instances of `foo` with `bar`, except in the second paragraph.
