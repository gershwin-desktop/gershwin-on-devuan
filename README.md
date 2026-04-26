# Gershwin on Devuan

Live ISO of the [Gershwin](https://github.com/gershwin-desktop/gershwin-developer) NeXTSTEP-style desktop running on a Devuan (sysvinit) base. Builds for amd64 and arm64.

## Build

CI builds amd64 + arm64 ISOs on every push to `main` and uploads them to the `continuous` release tag.

To build locally on a Devuan or Debian host:

```sh
sudo ./build.sh
```

Build deps: `debootstrap squashfs-tools xorriso mtools dosfstools grub-pc-bin grub-efi-amd64-bin grub-efi-arm64-bin`. The `ci/containers/Dockerfile` is the authoritative dep list.

## License

BSD 2-clause. See `LICENSE`.
