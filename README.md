# Northstar Client Linux OCI Images

Northstar has historically been inconsistent with running on Linux. This project aims to combine multiple community efforts into a single package to provide a nuclear option for running Northstar on Linux systems.

These images are designed to be used with distrobox to provide the best system integration out-of-the-box.

## Example Usage

```
$ distrobox-create --name northstar --image ghcr.io/cyrv6737/northstar-client-steam:latest
$ distrobox-enter -n northstar
$ steam
```
Set Titanfall 2 to run with NorthstarProton. Afterwards Northstar can be run with this one-liner assuming that your main instance of Steam is closed:
```
$ distrobox-enter -n northstar -- steam steam://rungameid/1237970
```
If EA App is displaying a blank window, run:
```
$ distrobox-enter -n northstar -- fix-ea-app
```

## TODO

- [X] Steam Images
    - [X] Install NorthstarProton by default
    - [X] Find a solution for EA App protonfixes
- [X] Install LatencyFleX by default
- [X] AMD Hardware
- [ ] Nvidia Hardware
- [ ] Non-steam Images