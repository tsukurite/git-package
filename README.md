# git-package

packaging files

## Installation

```console
$ cd `git --exec-path` && curl -OL https://raw.githubusercontent.com/tsukurite/git-package/master/git-package
```

## Usage

all my commit:

```console
$ git package --author=sasaplus1
```

today's my commit:

```console
$ git package --since=midnight --author=sasaplus1
```

latest 5 commits:

```console
$ git package HEAD~5..HEAD
```

all arguments pass to `git log`.

## License

The MIT license. Please see top of `git-package`.
