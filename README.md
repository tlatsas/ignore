ignore.py
---------

Get gitignore templates from the [github/gitignore][1] repository.
It supports listing and downloading available templates using the github API.

dependencies
------------

* python >= 3
* [requests][2]


examples
--------

List all available .gitignore templates:

    $ ignore.py list

Get vim, python and c .gitignore templates and print on `STDOUT`:

    $ ignore.py get vim python c

You can use a shell redirect to write the output in a .gitignore file or use the
`--output-files` and `--merge` options:

    $ ignore.py get -o -m vim python c

If a .gitignore file already exists you will be prompted to overwrite it unless
you use the `--force` option. For more information see `ignore.py -h`.

license
-------

See `COPYING`

[1]: https://github.com/github/gitignore
[2]: http://docs.python-requests.org/en/latest/
