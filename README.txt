# mass_rename

mass_rename is a simple utility to rename group of files with your favorite `$EDITOR`.

# Install

mass_rename can be installed with pip

```shell
$ sudo pip install mass_rename
```

# Terminal and Editor

mass_rename will launch your favorite (unless `-s` is specified, which will launch vim in split mode)
that will be read from your $EDITOR settings variable.

```bash
echo $EDITOR
```

# Usage

```
usage: mass_rename [-h] [-s] [-c] [-C] [-k] [-v] [-e EXTENSION]
  files [files ...]

Command line parser for Mass Rename

positional arguments:
  files                 List of files to be renamed

 optional arguments:
  -h, --help            show this help message and exit
  -s, --split           Open vim in split mode, edit in the left view (force
                        the use of vim instead of $EDITOR)
  -c, --confirm         Print changes and wait for confirmation
  -C, --confirm-all     Ask confirmation for each file
  -k, --skip-extension  Skip extensions
  -v, --verbose         Add verbosity
  -e EXTENSION, --extension EXTENSION
                        Extra extensions if not recognized (can be specified
                        more times)
```

# About
Author: Enrico Carlesso
License: [WTFPL](http://www.wtfpl.net/about/)

Thanks:

 - [vim](http://www.vim.org/) and all the Vim community

mass_rename has been tested with Python 3.3.2
