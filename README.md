# grunt-rollup

> Grunt plugin for [rollup](https://github.com/rollup/rollup) - next-generation ES6 module bundler

## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-rollup --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-rollup');
```

## The "rollup" task

### Overview
In your project's Gruntfile, add a section named `rollup` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  rollup: {
    options: {
      // Task-specific options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
});
```

### Options

Supports all the options from [rollup's JavaScript API](https://github.com/rollup/rollup/wiki/JavaScript-API) apart from sourcemaps.

### Usage Examples

```js
grunt.initConfig({
  rollup: {
    options: {},
    files: {
      'dest/bundle.js': ['src/entry.js'], // Only one source file is permitted
    },
  },
});
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).
