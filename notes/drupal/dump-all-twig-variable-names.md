# Dump all twig variable names in the current context

To see all available twig variable names on the current template, you can use `dump()` with the globally available `_context` variable:

```
{{ dump(_context|keys) }}
```

This is useful if you don't want to use Kint or other alternatives. See the [Drupal 8 documentation](https://www.drupal.org/docs/8/theming/twig/discovering-and-inspecting-variables-in-twig-templates) for more details.