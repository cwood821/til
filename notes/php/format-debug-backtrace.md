# Format debug_backtrace as JSON 

To produce a nicely formatted JSON representation of `debug_backtrace` results: 

```php
error_log(json_encode(debug_backtrace(DEBUG_BACKTRACE_IGNORE_ARGS | DEBUG_BACKTRACE_PROVIDE_OBJECT)));
```

This a slight variation of a snippet in a [great post]() on freek.dev.