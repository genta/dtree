# dtree

`dtree` is a utility to retrieve the specified directory tree.

`dtree` displays the files under specified directories, with the detailed
informations (file type, size, permissions, hash digest, etc.) of each file.

The main use case of `dtree` is compare the integrity of files between systems.
For examples, if the `dtree` output were same between local and remote system,
this means that the files under specified directory is actually same.

It's similar to `mtree(1)` in *BSD, but output of `dtree` is suitable to
compare using `diff`.

Also, this aims to be able to work on legacy UNIX like OS (e.g. Debian Squeeze,
VyOS Helium, etc.), without installing external libraries. This requires only
Perl 5.10.1 and Perl's standard modules.

## Usage

```
$ dtree /usr/local
```

## Installation

```
$ install -m 755 dtree /usr/local/bin
```

## Dependency

* Perl 5.10.1 or later

## License

The 2-Clause BSD License.
