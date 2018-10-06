# resume-cli

[![Gitter](https://img.shields.io/gitter/room/jsonresume/public.svg)](https://gitter.im/jsonresume/public)
[![Build status](https://img.shields.io/travis/rbardini/resume-cli.svg)](https://travis-ci.org/rbardini/resume-cli)
[![Dependencies status](https://img.shields.io/david/rbardini/resume-cli.svg)](https://david-dm.org/rbardini/resume-cli)
[![devDependencies status](https://img.shields.io/david/dev/rbardini/resume-cli.svg)](https://david-dm.org/rbardini/resume-cli?type=dev)
[![npm package version](https://img.shields.io/npm/v/@rbardini/resume-cli.svg)](https://www.npmjs.com/package/@rbardini/resume-cli)

A command line interface for [JSON Resume](https://jsonresume.org), compatible with the
bleeding edge [resume schema](https://github.com/jsonresume/resume-schema/tree/v1.0.0).

[Read more...](https://jsonresume.org/schema/)

## Donations (upstream)

[![Bountysource](https://www.bountysource.com/badge/team?team_id=21303&style=bounties_received)](https://www.bountysource.com/teams/jsonresume/issues)
[![tip for next commit](https://tip4commit.com/projects/43122.svg)](https://tip4commit.com/github/jsonresume/resume-cli)

## IRC

Use your favorite IRC client to join the `#jsonresume` channel on Freenode.  

Or instead, you can use the web client:  [http://webchat.freenode.net](http://webchat.freenode.net?channels=%23jsonresume).


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


## `resume register`

_Registration is optional._

To publish your resume to your account with a custom domain extension at 
http://registry.jsonresume.org. You will first need to acquire login credentials.

## `resume login`

To log into a registered account. This will allow you to publish with requiring you to reenter your credentials.


## `resume publish`


This command will guide you through the publish process.

Options:
  - `--theme <name>` Style your resume. (Default: `even`)


## `resume serve`

Starts a web server that serves your local `resume.json`.  

Options: 
  - `--port <port>`
  - `--theme <name>`

If no theme is specified, it will look for the file `index.js` and call 
`render()`. This is useful when developing themes.



# License

Available under [the MIT license](http://mths.be/mit).
