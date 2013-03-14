# rr - Move files or directores to Trash on a Mac

Use `rr` in place of `rm` on a Mac to remove a file or directory.
Instead of deleting it, it just moves it to the Trash.
This is nice for huge directory trees because it happens instantly.

Options:

`-f`

> When deleting a directory, force deletion of the existing
> ~/.Trash/{dirname} if there is already one in the trash.

## Installation

```sh
curl https://raw.github.com/BMorearty/rr/master/rr >> /usr/local/bin/rr
chmod +x /usr/local/bin/rr
```

## Usage

```sh
$ rr giant-directory-tree another-dir some-file etc
```

It just takes a fraction of a second, no matter how big the dir tree is,
because all it has to do is move the root.

Then, when you're ready, empty your Mac trash.

## Removal

```sh
rr /usr/local/bin/rr    # ;-)
```
