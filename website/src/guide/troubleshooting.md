# Troubleshooting

If you encounter any issues, then try the following.

## Check for Known Limitations

Check if your problem is already described on the [known limitations page](./troubleshooting/limitations), where you'll also find some suggested workarounds.

## Expand the Macro

Suppose you see a compile error coming from the code generated by a macro. The error message is not very informative because it points to some code inside of the macro that you don't see.

In this case, try expanding the macro using Rust Analyzer's command ["Expand macro recursively"](https://rust-analyzer.github.io/book/features.html#expand-macro-recursively). It works for any kind of macro including attribute macros.

Then copy the expanded code, delete the original macro invocation, and replace it with the expanded code. Compile your program again to see where exactly the error occurs.

**Example:**

<video controls src="/expand-macro-recursively.mp4" title="Title"></video>

## Open an Issue

If nothing else helps, feel free to [open an issue](https://github.com/elastio/bon/issues). We'll definitely figure this out 🐱.
