> ⚠️ Fork no longer maintained in favor of original [jsonresume/resume-cli](https://github.com/jsonresume/resume-cli) project. All changes have been merged to the upstream repository and released in version 2.0.0.

# @rbardini/resume-cli

[![Gitter](https://img.shields.io/gitter/room/jsonresume/public.svg)](https://gitter.im/jsonresume/public)
[![Build status](https://img.shields.io/travis/rbardini/resume-cli.svg)](https://travis-ci.org/rbardini/resume-cli)
[![Dependencies status](https://img.shields.io/david/rbardini/resume-cli.svg)](https://david-dm.org/rbardini/resume-cli)
[![devDependencies status](https://img.shields.io/david/dev/rbardini/resume-cli.svg)](https://david-dm.org/rbardini/resume-cli?type=dev)
[![npm package version](https://img.shields.io/npm/v/@rbardini/resume-cli.svg)](https://www.npmjs.com/package/@rbardini/resume-cli)

A command line interface for [JSON Resume](https://jsonresume.org), compatible with the
bleeding edge [resume schema](https://github.com/jsonresume/resume-schema/tree/v1.0.0).

[Read more...](https://jsonresume.org/schema/)


# Getting Started

Install the command-line tool:

```
npm install -g @rbardini/resume-cli
```


# Usage

## `resume --help`

Show a list of options and commands for the <abbr title="Command Line Interface">CLI</abbr>.


## `resume init`

Creates a new `resume.json` file in your current working directory.

Complete the `resume.json` with your text editor. Be sure to follow the schema 
(available at http://jsonresume.org).


## `resume test`

Validates your `resume.json` against our schema tests to ensure it complies with 
the standard. Tries to identify where any errors may be occurring.


## `resume export [fileName]`

Exports your resume locally in a stylized HTML, Markdown, or PDF format.

A list of available themes can be found here: http://jsonresume.org/themes/

Please npm install the theme you wish to use locally before attempting to export it.

Options:
  - `--format <file type>` Example: `--format pdf`
  - `--theme <name>` Example: `--theme even`

## `resume serve`

Starts a web server that serves your local `resume.json`.  

Options: 
  - `--port <port>`
  - `--theme <name>`

If no theme is specified, it will look for the file `index.js` and call 
`render()`. This is useful when developing themes.



# License

Available under [the MIT license](http://mths.be/mit).
