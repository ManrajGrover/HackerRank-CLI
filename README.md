# HackerRank-CLI
> CLI for running code using [HackerRank API](https://www.hackerrank.com/api).

## Install

Run the following command

```
$ npm install -g hackerrank-cli
```

## API Key

You can get your HackerRank API Key by visiting [HackerRank API](https://www.hackerrank.com/api) page.

## Usage

### Commands available

```
$ hackerrank <command>

Commands:
  run     Run code on HackerRank server
  config  Change config file

Options:
  -h, --help  Show help                                                [boolean]
```

#### Command `run`

```
$ hackerrank run <options>

Options:
  -h, --help      Show help                                            [boolean]
  -s, --source    Source Code file path                               [required]
  -i, --input     Input file path                                     [required]
  -l, --language  Language. Change `config` for default.
  -o, --output    Output file path                                    [required]

Examples:
  hackerrank run -s A.cpp -i Input00.in -o Output.txt -l 2
```

#### Command `config`
Run `$ sudo hackerrank config` to change configuration of your installation. This includes default language and API Key.

```
$ sudo hackerrank config [options]

Options:
  -h, --help  Show help                                                [boolean]
  -l, --list  List language and their code                             [boolean]

Examples:
  sudo hackerrank config -l
```

## License

MIT © [Manraj Singh](https://github.com/ManrajGrover)
