# Is it cloudy? 🌦

Node command line tool to printing weather info.

<p align="center"><img width="551" alt="Bash prompt with weather info" src="https://cloud.githubusercontent.com/assets/141232/23497068/0d46f7dc-ff54-11e6-88e5-9ca9ff9180e7.png"></p>

## Installation

```sh
npm install -g is-it-cloudy
```

## Usage

```
  Usage: is-it-cloudy [options]

  Options:

    -h, --help         output usage information
    -V, --version      output the version number
    --city [city]      City name
    --appid [id]       App id for openweathermap.org
    -f, --fetch        Do not check mtime, fetch every time
    --format [format]  Format output, %e for emoji, %t for temp
```

## Example

You can use this command to display weather in bash prompt.

```sh
function set_ps1 {
	PROMPT_WHEATHER=$(is-it-cloudy --format '%e %t');
  export PS1="${PROMPT_WHEATHER} \w\$"
}

export PROMPT_COMMAND="set_ps1;"
```

## License

MIT
