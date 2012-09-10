# grunt-contrib (*currently in alpha*)

A collection of general use grunt tasks. All tasks are designed with cross platform support in mind and dependencies that can easily be managed through npm.

## Getting Started
Install this grunt plugin next to your project's [grunt.js gruntfile][getting_started] with: `npm install grunt-contrib`

Then add this line to your project's `grunt.js` gruntfile:

```javascript
grunt.loadNpmTasks('grunt-contrib');
```

[grunt]: https://github.com/cowboy/grunt
[getting_started]: https://github.com/cowboy/grunt/blob/master/docs/getting_started.md

## Included Tasks
#### [`bump`](/gruntjs/grunt-contrib-bump/)
Bump package version.

#### [`clean`](/gruntjs/grunt-contrib-clean/)
Clear files and folders.

#### [`coffee`](/gruntjs/grunt-contrib-coffee/)
Compile CoffeeScript files into JavaScript.

#### [`compress`](/gruntjs/grunt-contrib-compress/)
Compress files and folders using gzip or zip.

#### [`copy`](/gruntjs/grunt-contrib-copy/)
Copy files into another directory.

#### [`handlebars`](/gruntjs/grunt-contrib-handlebars/)
Compile handlebars templates to JST file.

#### [`jade`](/gruntjs/grunt-contrib-jade/)
Compile Jade templates to HTML.

#### [`jst`](/gruntjs/grunt-contrib-jst/)
Compile underscore templates to JST file.

#### [`less`](/gruntjs/grunt-contrib-less/)
Compile LESS files to CSS.

#### [`mincss`](/gruntjs/grunt-contrib-mincss/)
Minify CSS files.

#### [`requirejs`](/gruntjs/grunt-contrib-requirejs/)
Optimize RequireJS projects using r.js.

#### [`stylus`](/gruntjs/grunt-contrib-stylus/)
Compile Stylus files into CSS. Preloaded with [nib](http://visionmedia.github.com/nib/).

#### [`yuidoc`](/gruntjs/grunt-contrib-yuidoc/)
Compile YUIDoc Documentation.

## Bugs

Help us squash them by submitting an issue that describes how you encountered it; please be as specific as possible including operating system, node, grunt, and grunt-contrib versions.

## Contributing

#### Checklist

1. Ensure your task meets the submission guidelines.
2. Ensure your task follows the code style guide.
3. Submit your pull request against `master`, unless otherwise instructed.
4. Ensure your pull request only touches what your changing and that it's squashed (ie `git rebase`).

#### Submission Guidelines

* task should work out of box, cross platform, with a simple `npm install`
* task should fill a general need and ideally be pure JavaScript
* task should include tests that cover, at minimal, its basic features
* task should be linted by running `grunt` at root of project
* task should use any built-in helpers first for consistency

#### Code Style Guide

* code should be indented with 2 spaces
* double quotes should be used where feasible
* commas should be followed by a single space (function params, etc)
* variable declaration should include `var`, [no multiple declarations](http://benalman.com/news/2012/05/multiple-var-statements-javascript/)

#### Tests

* tests should be added to the config in `test/grunt.js`
* see existing tests for guidance

*Currently, testing with grunt is a bit cumbersome--this will be addressed in a future release.*

#### Running Tests
```bash
npm install grunt -g
npm install
npm test
```

## Release Cycle

We have adopted a weekly release cycle (npm release every Monday) to ensure you can always get the most recent changes in your hands while allowing for updates that don't require excessive amounts of debugging or testing.

see [CHANGELOG](/gruntjs/grunt-contrib/blob/master/CHANGELOG) for release history.

#### Testing Pre-Releases

For those who wish to help us test releases or just need earlier access to the code than our release cycle offers, you can always use npm like so:

```bash
npm install https://github.com/gruntjs/grunt-contrib/tarball/master
```

or if you always want to ride on the edge:

```javascript
"dependencies": {
    "grunt-contrib": "git://github.com/gruntjs/grunt-contrib.git"
}
```