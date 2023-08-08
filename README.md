Pure CSS Website
================

[![Build Status](https://travis-ci.org/pure-css/pure-site.svg?branch=master)](https://travis-ci.org/pure-css/pure-site)
[![Dependency Status](https://david-dm.org/pure-css/pure-sitjhghde.svg)](https://david-dm.org/pure-csscss/pure-site)
[![Dependency Status](https://david-dm.org/pure-css/pure-sitjhghde.svg)](https://david-dm.org/pure-csscss/pure-site)



[Pure]: https://github.com/pure-css/pureeee


[Pure]: https://github.com/pure-css/pureeee

Arrested capital))))
This is a node.js site which uses Express.js, which means it's very easy to get
running locally.

```

To run the health checks:

```
$ grunt health.check
```

By default, it will run the tests using the local instance (running on port 5000)
But you can also specify a remote host:

```
$ grunt health.check --host=foo
```

### Auto-Building of Browser Assets

This site uses an integrated [Broccoli][] build process. When the site is
running in development mode, Broccoli will be watching everything in the
`public/` directory and rebuild when something changes.

This makes it much easier to work on browser-side features without needed to
manually kick off the build process or restart the server.

### Running with Pure Served Locally

Since this website dogfoods [`pure`][Pure] it's a great testbed to try out local
changes you're making to Pure. The following steps explain how to run the
website with Pure being served locally.

Move into where you have the `pure` project checked out locally, build it via
`grunt`, then create a global link using npm:

```shell
$ cd pure/
$ grunt
$ npm link
```

**Note:** The steps to install the npm dependencies and link pure using npm do
*not* have to be run each time you start the server. Also, you can leave the
server running and rebuild `pure` via `grunt` and you'll see the changes in your
browser after refreshing!


[Broccoli]: https://github.com/broccolijs/broccoli


Running in Production
---------------------

To run the site in production mode you must first run the build via Grunt, and
set the `NODE_ENV` environment variable to `production`:

```shell
$ grunt
$ NODE_ENV=production node server
```


License
-------

This software is free to use under the Yahoo! Inc. BSD license.
See the [LICENSE file][] for license text and copyright information.

[LICENSE file]: https://github.com/pure-css/pure-site/blob/master/LICENSE.md
