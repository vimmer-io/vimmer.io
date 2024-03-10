You can search in Vim by hitting the `/` or `?` keys in normal mode, which initiate a forward and backward search respectively. These searches operate on the _entire buffer_ — and usually, this is what you want.

But what if you want to limit your search to a particular range of lines? For example, suppose you've got a large log file and you want to search for a particular term within a specific line range.

There are a few ways to do this, but it's usually easiest to take a visual selection of the 'interesting' lines, and use the `\%V` regex atom. This atom limits matches to _within the visual area_, so instances of the pattern outside of the visual area aren't picked up. So, if you wanted to search for the word `foo` within a bunch of lines, you would:

- visually select the lines with visual-line mode (`V`)
- re-enter normal mode (`<esc>`)
- initiate a forward search (`/`)
- use the `\%Vfoo` search pattern

**Let's try it in the editor.** Search for the word `foo` within the interesting line range by following the instructions above.
