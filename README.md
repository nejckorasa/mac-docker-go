# mac-docker-go

Script to make your life easier with Docker daemon on MacOS.

It supports:
- starting/restarting/status of Docker demon
- killing/removing Docker containers, images
- pruning images. volumes, networks...


## Install

```console
$ brew install nejckorasa/tap/dckr
```

See [homebrew-tap](https://github.com/nejckorasa/homebrew-tap)

## Usage

```bash
Start/stop docker daemon and kill/remove/stop/prune containers, images, volumes...
Usage: dckr [options]

Options:
  k     | --kill                 Kill daemon
  s     | --start                Start daemon
  r     | --restart              Restart daemon
  ds    | --status               Status of daemon

  ka    | --kill-all             Kill all running containers
  sa    | --stop-all             Stop all containers
  rma   | --remove-all           Remove all containers
  rmai  | --remove-all-images    Remove all images

  ip    | --image-prune          Remove dangling images
  ipa   | --image-prune-all      Remove all unused images
  vp    | --volume-prune         Remove all unused volumes
  np    | --network-prune        Remove all unused network
  sp    | --system-prune         Remove all unused objects

  -h                             Display help
```


## Some Examples

Restart docker daemon:

```console
$ dckr r
```

Kill docker daemon:

```console
$ dckr k
```

Stop all containers:

```console
$ dckr sa
```

Removing all containers:

```console
$ dckr rma
```

Removing all images:

```console
$ dckr rmai
```

See [Usage](#Usage) for all options
