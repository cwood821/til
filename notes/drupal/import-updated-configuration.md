# Import updated configuration without uninstalling module

To import updated configuration from yaml files without uninstalling and re-installing a module, use the Drush `config-import` (`cim`) command:

```
drush cim -y --partial --source=modules/custom/my_modul_name/config/install/
```

This is useful for refreshing migrations without uninstalling. Hat tip to the [Phase2Technology blog](https://www.phase2technology.com/blog/drupal-8-migrations).

Also, see [drush command page](https://drushcommands.com/drush-8x/config/config-import/).


