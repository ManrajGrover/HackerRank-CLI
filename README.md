# HackerRank-CLI
[![Build Status](https://travis-ci.org/manrajgrover/HackerRank-CLI.svg?branch=master)](https://travis-ci.org/manrajgrover/HackerRank-CLI) [![npm version](https://badge.fury.io/js/hackerrank-cli.svg)](https://www.npmjs.com/package/hackerrank-cli) [![npm](https://img.shields.io/npm/dt/hackerrank-cli.svg)](https://www.npmjs.com/package/hackerrank-cli) ![awesome](https://img.shields.io/badge/awesome-yes-green.svg)
> CLI for running code using [HackerRank API](https://www.hackerrank.com/api).

## Demo

![Demo](https://raw.githubusercontent.com/manrajgrover/HackerRank-CLI/master/assets/demo.gif)

## Install

Run the following command

```sh
$ npm install -g hackerrank-cli
```

## API Key

You can get your HackerRank API Key by visiting [HackerRank API](https://www.hackerrank.com/api) page.

## Usage

### Commands available

```sh
$ hackerrank <command>

Commands:
  run     Run code on HackerRank server
  config  Change config file

Options:
  -h, --help  Show help                                     [boolean]
```


#### Command `run`

```sh
$ hackerrank run <options>

Options:
  -h, --help      Show help                                 [boolean]
  -s, --source    Source Code file path                    [required]
  -i, --input     Input file path                          [required]
  -l, --language  Language. Change `config` for default.
  -o, --output    Output file path                         [required]

Examples:
  hackerrank run -s A.cpp -i Input00.in -o Output.txt -l 2
```


#### Command `config`
Run `$ sudo hackerrank config` to change configuration of your installation. This includes default language and API Key.

```sh
$ sudo hackerrank config <options>

Options:
  -h, --help  Show help                                     [boolean]
  -l, --list  List language and their code                  [boolean]

Examples:
  sudo hackerrank config -l
```

## Development

Run:

```sh
$ git clone https://github.com/manrajgrover/HackerRank-CLI.git
$ cd HackerRank-CLI
$ npm link
```

This will setup a symbolic link to the CLI. Any changes in source files will now be reflected when running the `hackerrank` command.

To lint your code, run

```sh
$ npm run lint
```

## License

[MIT](https://github.com/manrajgrover/HackerRank-CLI/blob/master/LICENSE) © [Manraj Singh](https://github.com/manrajgrover)
