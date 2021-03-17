# ISO Date strings without timezones are interpreted differently across browsers

Date strings in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format that leave off a timezone might be interpreted differently depending on the browser when instantiating a Date object.

Firefox and Chrome (at time of writing) will intepret strings missing timezones as originating in the user's timezone, Safari will interpret those strings as originating from timezone z (utc+-00:00). 

Firefox:
```js
new Date("2020-08-26T22:10:31") // no timezone, string is interpreted as from users locale 
// Wed Aug 26 2020 22:10:31 GMT-0500 (Central Daylight Time)

new Date("2020-08-26T22:10:31Z") // Interpreted with timezone as a date string from Z (utc+-00:00)
// Wed Aug 26 2020 17:10:31 GMT-0500 (Central Daylight Time)
```

Safari (13.1.2):
```js
new Date("2020-08-26T22:10:31") // no timezone, string is interpreted as from timezone Z (utc+-00:00)
// Wed Aug 26 2020 17:10:31 GMT-0500 (CDT)

new Date("2020-08-26T22:10:31Z") // with timezone, is interpreted as from timezone Z (utc+-00:00)
// Wed Aug 26 2020 17:10:31 GMT-0500 (CDT)
```
