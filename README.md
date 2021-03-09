# Gregors Script Library

**THIS IS WORK IN PROGRESS!** Come back in a few days.

None of the files are executable, and none have a shebang at the beginning
because they are not shell scripts but collections of functions that need
to be sourced. This way it's possible to manipulate variables in the current
shell environment.

## Usage

```shell
git clone https://github.com/gregor-j/gregors-script-library.git "/path/to/gregors-script-library"
```

Add the loader to your shell init script, like `/etc/bash.bashrc`.

```shell
export SCRIPT_LIBRARY="/path/to/gregors-script-library/lib"
. "${SCRIPT_LIBRARY}/loader.function"
```

Load some scripts from the library...
