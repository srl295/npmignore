# npmignore [![NPM version](https://badge.fury.io/js/npmignore.svg)](http://badge.fury.io/js/npmignore)

> Command line tool for creating or updating a .npmignore file based on .gitignore.

## Install
### Install globally with [npm](npmjs.org):

```bash
npm i -g npmignore
```

## Run tests

```bash
npm test
```

## Usage

Say `.gitignore` has:

```bash
node_modules
test/actual
```

And you want `.npmignore` to have:

```bash
node_modules
test/actual
test/fixtures
```

In the command line run:

```bash
npmignore "test/fixtures"
```

An `.npmignore` file will be created, or updated:

```bash
node_modules
test/actual

# npmignore
test/fixtures
```

**Heads up!**

The `# npmignore` comment is used to ensure that `.npmignore` reflects the latest changes in your `.gitignore` file, just by running `npmignore` in the command line.

_If you want to preserve everything in your `.npmignore` file, regardless of what is in `.gitignore`, just add the `# npmignore` comment at the top of the `.npmignore` file.

## Contributing
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/npmignore/issues).

## Author

**Jon Schlinkert**
 
+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert) 

## License
Copyright (c) 2014 Jon Schlinkert, contributors.  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on October 26, 2014._