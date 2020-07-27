# Send copied text to OS clipboard

On MacOS, you can rebind the Enter key in tmux configuration to send copied text to `pbcopy`:

```
bind -T copy-mode-vi Enter send-keys -X copy-pipe-and-cancel "pbcopy"
```

See [this article](https://www.freecodecamp.org/news/tmux-in-practice-integration-with-system-clipboard-bcd72c62ff7b/) for more information and other operating systems.

