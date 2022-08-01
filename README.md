# BookOff Search Redirect

You can't add a BookOff search to modern browsers because their URL parameters
aren't UTF-8 encoded - they're SJIS hex-encoded, then re-encoded so all the
percent signs become `%25`. This repo contains a page that takes normal query
paramters and re-encodes them.

To use this, add a custom search with a query string like this:

```
https://demo.cotonoha.io/bookoff/bookoff.html?q=%s
```

After navigating to that page, you'll be redirected to a bookoff search with
the correct URL.

[encoding.js](https://github.com/polygonplanet/encoding.js/) is used under the
terms of the MIT license.

The code in this library is public domain / WTFPL. 
