# Northstar Client Linux OCI Images

Northstar has historically been inconsistent with running on Linux. This project aims to combine multiple community efforts into a single package to provide a nuclear option for running Northstar on Linux systems.

These images are designed to be used with distrobox to provide the best system integration out-of-the-box.

## Example Usage

```
$ distrobox-create --name northstar --image ghcr.io/cyrv6737/northstar-client-steam:latest
$ distrobox-enter -n northstar
$ steam
```

## TODO

- [ ] Steam Images
    - [X] Install NorthstarProton by default
    - [ ] Find a solution for EA App protonfixes
- [X] Install LatencyFleX by default
- [X] AMD Hardware
- [ ] Nvidia Hardware
- [ ] Non-steam Images