# git-snap

## Build

Tested on Ubuntu 22.04.

### Prerequisites

```
sudo apt install snap snapcraft
```

### Build

On the first build, let it install and configure `lxd`, if missing. If the automatic configuration fails and the error says 'manual configuration is required', run:
```
sudo lxd init
```

Make sure to pick a subnet that is not in use.

[Build providers - snapcraft.io](https://snapcraft.io/docs/build-providers)

Build the snap:
```
snapcraft
```

## Install

```
sudo snap install --devmode git-bszakaly_0.1_amd64.snap
```

## Run

```
git-bszakaly.git --version
```