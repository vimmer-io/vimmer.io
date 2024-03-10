You probably already new that you can use the `^` key to jump to the first non-blank character of a line. You probably also think that `^` is a little hard to type. Did you know that there's a more ergonomic alternative?

The `_` key in normal mode does _almost_ the same thing. If you're in normal mode, hitting `^` is the exact same as hitting `^`. I personally find it a lot easier to reach for `_`, though, because I'm so much more used to typing it.

`_` is slightly different in other contexts though.

- `_` is a linewise motion, compared to `^` which is a characterwise motion — `d_` will delete the entire line, where `d^` will delete from the current cursor position to the first non-blank character.
- `_` accepts a count, where `^` doesn't.
