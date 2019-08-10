# mac-docker-go

Script to make your life easier starting/restarting/killing Docker daemon on MacOS. It is *not* written in Go.

```
Usage: dckr [options]

Options:
  -k  | --kill        Kill Docker daemon
  -s  | --start       Start Docker daemon
  -r  | --restart     Restart Docker daemon
  -ka | --killall     Kill all running Docker containers
  -h                  Display help

  Defaults to restart if no options are present

```


Example usage:

```bash
$ dckr
```

or killing all running containers:

```bash
$ dckr -ka
```


#### Install

```
$ brew install nejckorasa/tap/dckr
```

See [homebrew-tap](https://github.com/nejckorasa/homebrew-tap)
