# Get URL of current page in Drupal Twig

The `url` function when passed `<current>` will return the URL of the current page:

```twig
{% set cur_page_url = url("<current>") %}
```

Note: This will return a render array. To get at the value, you might use the [render filter](https://www.drupal.org/docs/8/theming/twig/filters-modifying-variables-in-twig-templates#render) or access its markup as an array index:

```twig
{% set cur_page_url = url("<current>") %}

{{ cur_page_url|render }}
{{ cur_page_url["#markup"] }}
```

Drupal 8 has other [Twig extensions](https://www.drupal.org/docs/8/theming/twig/functions-in-twig-templates) available in core.
