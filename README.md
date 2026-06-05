# tofu60 ZMK config

Local build environment for the Polarity Works BT60 v2 config.

## Build

Enter the direnv shell:

```sh
direnv allow
```

Build the firmware:

```sh
zmk-build-tofu60
```

The firmware is copied to:

```sh
bt60_v2.uf2
```

You can also build without direnv:

```sh
nix run path:.#build
```

## Flash

Put the keyboard into bootloader mode, then copy `bt60_v2.uf2` onto the mounted bootloader drive.
