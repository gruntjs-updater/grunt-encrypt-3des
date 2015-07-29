# grunt-encrypt

> Encrypt your files with Grunt, crypto-js and 3des

## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-encrypt-3des --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-encrypt-3des');
```

## The "encrypt" task

### Overview
In your project's Gruntfile, add a section named `encrypt3des` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  encrypt3des: {
    options: {
      key: grunt.cli.options.key,
      dest: output/encrypted/'
    },
    file: 'path/to/file'
  },
});
```

### Options

#### options.key
Type: `String`
Default value: `null`

A string value used to encrypt a file

#### options.dest
Type: `String`

A string to the output directory, defaults to the source file path

#### options.ext
Type: `String`
Default value: `null`

A string to set the file extension for the encrypted file.

#### file
Type: `String`

Path to file to encrypt.

#### files
Type: `Object`

An object containing a map of files.

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
- 2015-07-29 v0.1.0 Initial release