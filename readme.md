# Opal Example

## Dependencies

Downloaded opal and opal-parser from cdn and placed in js/ folder.
```
$ cd public/js/
$ wget https://cdn.opalrb.com/opal/current/opal.js
$ wget https://cdn.opalrb.com/opal/current/opal-parser.js
```

Compiled opal-browser dependencies from https://github.com/opal/opal-browser like so
```
$ cd ../opal-browser/
$ opal -I ./opal --gem paggio --compile opal/browser.rb > browser.js
$ opal -I ./opal --gem paggio --compile opal/browser/http.rb > http.js
```

and copied the JS files to this projects public/js/ folder.

## Run Server
```
$ ruby server.rb
```
and navigate to http://localhost:8080 in browser.