# Turn off exception handling in Laravel tests

To turn off exception handling in a Laravel test, use the `withoutExceptionHandling` method.

```php
$this->withoutExceptionHandling();
```

This is available since Laravel 5.5. It's handy to debug and see issues inside your test results. 

For more discussion, see [this discussion thread](https://laracasts.com/discuss/channels/testing/help-me-understand-withexceptionhandling-and-withoutexceptionhandling);
