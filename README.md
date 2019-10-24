# mpick

## About
A small fuzzy search tool for the terminal, written in python.

## Usage
mpick reads in a list from stdin, after using the fuzzy search to select something, that selection
is output onto stdout.

```sh
# rerun a previous command:
$ eval $(fc -ln | mpick)
# switch to another wifi-network
$ find /etc/netctl/ -maxdepth 1 -type f -printf %f\\n | mpick | xargs sudo netctl switch-to
```

## Requirements

Python 3.X
