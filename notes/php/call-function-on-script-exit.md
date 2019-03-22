# Call a function on script exit with `register_shutdown_function`

To call a function on script exit, use the `register_shutdown_function` in PHP.

```php

function shutdown_handler() {
    // Send an email, notification, etc.
}

register_shutdown_function("shutdown_handler");
```

See the [official documentation](https://secure.php.net/manual/en/function.register-shutdown-function.php), as well as [some Stack Overflow](https://stackoverflow.com/questions/4410632/handle-fatal-errors-in-php-using-register-shutdown-function) [posts](https://stackoverflow.com/questions/13499399/explanation-of-register-shutdown-function). 
