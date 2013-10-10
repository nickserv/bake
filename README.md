# Bake
A simple make-like task runner that uses standard bash syntax. Bake organizes
tasks similary to make, but uses regular bash for variables, if statement, and
other constructs.

## Features
- Standard bash syntax. Why spawn shells on every line of code and add
  complicated variables when you can just write bash?
- Tasks can have prerequisites, as in make.
- Portable source code, written in bash.
- I am considering adding zsh support in the future.
- Useful features borrowed from rake:
  - List tasks in a Bakefile.
  - Intelligently search for Bakefiles in parent directories when running bake.

## Syntax
```
MESSAGE="Hello, world!"

speak:
  echo $MESSAGE
  echo "It is now `date`"
```
