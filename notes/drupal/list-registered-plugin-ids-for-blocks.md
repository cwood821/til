# List all registered plugin IDs for blocks with Drush

Sometimes you will need to reference blocks by their plugin ID. To list all registered plugin IDs for blocks via Drush, use the following snippet:
```
drush ev "print_r(array_keys(\Drupal::service('plugin.manager.block')->getDefinitions()));"
```

Credit to the [Twig Tweak](https://www.drupal.org/docs/8/modules/twig-tweak/rendering-blocks-with-twig-tweak) module documentation for this snippet.