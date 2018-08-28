# Pass data to all views with `res.locals` object

If you have data that is used by every view in your [Express](https://expressjs.com/) app, you can pass that data via the `res.locals` object.

```js
app.use(function(req, res, next) {
    res.locals.user = req.user;
    next();
});
```
This snippet from [Stackoverflow](https://stackoverflow.com/questions/15057857/node-js-express3-middleware-to-add-render-data-to-all-render-requests).

The `res.locals` object merges with other data [on render](https://github.com/expressjs/express/blob/3.1.0/lib/application.js#L467-474). See [the documentation](https://expressjs.com/en/api.html#res.locals) for more detail.

