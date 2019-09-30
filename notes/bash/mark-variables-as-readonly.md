# Mark variables as readonly in bash

In a Bash script, you can prevent variables from being reassigned by marking them `readonly`.

```bash
readonly MY_VAR='the_value'
```

In practice, this works like a constant in other languages. See [the documentation](https://www.gnu.org/software/bash/manual/html_node/Bourne-Shell-Builtins.html#index-readonly).
