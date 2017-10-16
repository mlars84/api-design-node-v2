# Front End Masters: API Design with Node V2
> Learn to build with Node, Express, Mongo, and GraphQL

## What you'll need to know
* JavaScript
* basic HTTP knowledge
* basic API knowledge

## Dependencies
* Mongo (if you don't have this, signup for a free mongo DB [at mLab](https://mlab.com/))
* Node 6+
* Yarn or Npm (Yarn recommended)

## Getting Started
The curriculum is broken up by branches. Each branch walks through a different lesson. There are usually some tests you must get to pass. For each branch, there is a solution branch.

* Checkout to the first lesson branch `git checkout lesson-1`

## Contributing
If you see issues:

* fork this repo
* clone your fork
* cut a branch
* write your code
* issue PR to upstream# Notes
- Why Express?
 - the go to for creating API's with node
 - other frameworks are based off express
 - tons of plugins and integrations
 - plenty of resources
 - easy to use
 - fast to develop
 - easy to test

- Features
 - declarative routing
   - exact, pattern, glob(splat, *), parameter matching
 - Middleware
   - functions to run serially on your requests
 - powerful response options
   - from JSON to static files
   - stream
   - redirects
 - DB agnostic
 - Highly configurable

- Hot Module Loading
 ```
 if (module.hot) {
    module.hot.accept(['./server'], () => {
 	 server.removeListener('request', currentApp)
 	 server.on('request', app)
 	 currentApp = app
    })
 }
 ```
- `app.all('*', (req,res) => res.json({ok: true}) )`
- Comes from webpack config and allows `hot` param on `module`

### Routing with Express
 - Flexible pattern matching
 - handles parameters
 - multi-router support
 - static & dynamic configuration
 - support for all HTTP verbs (only applies to REST)
 - order based
 - mount different routers on different paths that have different purposes



