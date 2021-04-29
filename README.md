# Shell Script Library

**THIS IS WORK IN PROGRESS!** Come back in a few days.

These are not executable files but collections of functions that need to be sourced.
This way it's possible to manipulate variables in the current shell environment.

## Usage

Clone the shell script library repository and source the loader script.

```shell
git clone https://github.com/gregor-j/shell-script-library.git
cd shell-script-library
export SCRIPT_LIBRARY=$(pwd)
. loader.function
```

For a more permanent solution add the loader to your shell init script, like `/etc/bash.bashrc`.

```shell
export SCRIPT_LIBRARY="/path/to/shell-script-library"
. "${SCRIPT_LIBRARY}/loader.function"
```

Now load some scripts from the library...

```shell
load common
printf '%bhello%b %bworld%b!\n' "$(color green)" "$(color reset)" "$(color bold red on yellow)" "$(color reset)"
```
