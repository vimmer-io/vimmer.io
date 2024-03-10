You can use the `?` key in normal mode to initiate a backwards search. This is the same as searching with `/`, but moving through the file backwards instead of forwards.

This is useful when the string that you're searching for contains `/` characters, because you don't have to escape them in the way you would if you were doing a forward search.

**Try it in the editor.** Search for the string `https://vimmer.io` using a forward search first, and notice that it's a bit of a pain because you have to escape the `/` characters. Then try searching for the same string with `?`. It's much easier!
