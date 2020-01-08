# Delete text without overwriting yanked text

To delete something without placing it into a register: 

```
"_dd
```

`"` sets the register, `_` is a blackhole. See [documentation](http://vimdoc.sourceforge.net/htmldoc/change.html#registers).

Hat tip to [Stack Overflow](https://stackoverflow.com/questions/3638542/any-way-to-delete-in-vim-without-overwriting-your-last-yank)


