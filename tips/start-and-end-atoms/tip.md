The start and end atoms, `\zs` and `\ze`, allow you to define where your match _starts_ and _ends_ respectively within your Vim search pattern. They're a way that you can tell Vim "hey, I want you to search for _this whole pattern_, but I only want you to _match_ this portion"

If you search for something like `foo\zsbar\zebaz`, your search pattern will only match the `bar` part of the word in `foobarbaz`.

This is particularly useful with substitutions — the `/baz.*\zsfoo` search pattern will match the last instance of `foo` on a line that has the word `baz` first, so hopefully you can see how these make complex substitutions quite simple.

**Try it in the editor!**
