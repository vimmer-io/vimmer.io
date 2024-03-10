Windows in Vim allow you to have multiple buffers visible on your screen at once. Tabs are just a collection of windows. If you've got multiple windows open, you might want to focus on _just one_ so that you can take a closer look. We can achieve this with tabs.

One of the best ways to do this is by using `:tab sp`, which takes your current window and opens it in a new tab. When you're done, your previous tab will have the windows in the same way you left them.

Here's how `:tab sp` works:

- `:sp` is a command that splits the current window horizontally
- `:tab` is a special command that _accepts another command_, and opens a new tab for each new window that that command creates

So under the hood, Vim is creating a new split, then immediately moving it to a new tab. This has the effect of 'zooming in' to a window temporarily.

Once you're done, you can close the new tab with `:tabc`.

**Let's try it in the editor.** There are three files: `demo` (which is already open), `demo_a.txt`, `demo_b.txt`, and `demo_c.txt`. Open then in different windows with `:sp demo_a.txt`, `:sp demo_b.txt`, and `:sp demo_c.txt`. Once you've got a window layout you're satisfied with, try 'breaking out' one of the windows with `:tab sp`!
