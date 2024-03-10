Vim has a built-in operator for formatting text. You can customise the behaviour of this operator with the `formatexpr` and `formatprg` options, but by default it's used for hard-wrapping text.

To use the format operator, you can either use:

- `gq` in normal mode, followed by a text object or a motion (if you're not sure what this means, check out [our lesson](https://vimmer.io/lesson/operators-motions-and-text-objects))
- `gq` in visual mode

**Try it in the editor.** The example text is hard-wrapped inconsistently. Try using the format operator to tidy it up!
