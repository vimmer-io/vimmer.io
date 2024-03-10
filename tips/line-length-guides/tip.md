Some programming languages recommend that your line length should be _below_ a certain threshold. Python, for example, [recommends that lines should not exceed 79 characters](https://www.python.org/dev/peps/pep-0008/).

Vim has an option called `colorcolumn` that lets us highlight a particular common inside a buffer. This makes it easy to see when we're spilling over the line length recommendations.

For Python, we'd want to enable it at column 80 — since everything beyond and including column 80 is undesirable. To do this, we can use the command `:set colorcolumn=80`.

**Let's try this in the editor.** The editor is pre-populated with some Python code. Enable the `colorcolumn` option at line 80 and see which lines are spilling over the boundary.
