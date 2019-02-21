# Append query parameters to pagination links in Laravel

To append query parameters (e.g. `?q=some-term`) to pagination links in Laravel, use the appends method to pass the current request query:

```
{{ $posts->appends(request()->query())->links() }}
```
 
This snippet is useful in situations when you are apply filters to paginated results via query parameters. See further conversation on [Stack Overflow](https://stackoverflow.com/questions/24891276/how-to-automatically-append-query-string-to-laravel-pagination-links/41976594#41976594).
