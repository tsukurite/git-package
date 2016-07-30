# git-package

package to changed files

## Installation

```console
$ cd "`git --exec-path`"
$ [sudo] curl -OL https://raw.githubusercontent.com/tsukurite/git-package/master/git-package
$ [sudo] chmod +x git-package
```

or

```console
$ git clone http://github.com/tsukurite/git-package.git
$ ln -s "`pwd`"/git-package/git-package "`git --exec-path`"
```

## Usage

all sasaplus1's commit:

```console
$ git package --author=sasaplus1
```

today's my commit:

```console
$ git package --since=midnight --author=`git config --get user.name`
```

since 2015-03-03:

```console
$ git package --date=local --since="2015-03-03"
```

latest 5 commits:

```console
$ git package HEAD~5..HEAD
```

all arguments pass to `git log`. if you want to know other options, execute `git log --help`.

## License

The MIT license. Please see top of `git-package`.
