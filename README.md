# vscode-indent-on-empty-line README

When the cursor moves to an empty line, automatically indent to the correct level.

That is, moving the cursor onto an empty line with the up/down/left/right arrows will cause the cursor to also jump to an appropriate level of indentation. This is influenced by the indentation settings for the language you're working in, but falls back to using the indentation level of the next non-empty line.

## Fork Changes

This fork changes the implicit indent behavior so it only runs when the active editor has unsaved changes.

## Configuration

This plugin adds the following movement commands and binds them to the arrow keys by default, overriding the corresponding builtin movement commands:

- `implicit-indent.cursorUp`
- `implicit-indent.cursorDown`
- `implicit-indent.cursorLeft`
- `implicit-indent.cursorRight`

It also binds to the following events

- `onStartupFinished`

If you wish to use different keys for these (such as vim-style keys), you can rebind those commands to different keys in your personal keyboard settings.
