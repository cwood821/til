# Run Laravel test without firing events

To prevent events firing while running tests, which may have side-effects, use the `withoutEvents` helper method:

```php
// Inside test code
$this->withoutEvents();
```

Laravel also provides a way to [fake events](https://laravel.com/docs/5.7/mocking#event-fake);
