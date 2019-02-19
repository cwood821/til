# Create model, controller, and migration in one artisan command

When using the `make:model` artisan command, use the `-mcr` flags to create a migration and resourceful controller, as well.

```
php artisan make:model Post -mcr
```

Hat tip to [Stack Overflow](https://stackoverflow.com/questions/43187735/laravel-5-4-create-model-controller-and-migration-in-single-artisan-command#43187825). In newer versions of Laravel, you can use the `-a` flag to do the same.
