# Shell Script Library

**THIS IS WORK IN PROGRESS!** Come back in a few days.

These are not executable files but collections of functions that need to be sourced.
This way it's possible to manipulate variables in the current shell environment.

## Usage

```shell
git clone https://github.com/gregor-j/shell-script-library.git "/path/to/shell-script-library"
```

Add the loader to your shell init script, like `/etc/bash.bashrc`.

```shell
export SCRIPT_LIBRARY="/path/to/shell-script-library"
. "${SCRIPT_LIBRARY}/loader.function"
```

Now load some scripts from the library...

```shell
load common
echo -e "$(color green)hello $(color bold red on yellow)world$(color reset)!"
```
