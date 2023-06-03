# IllusionX kernel for Pixel 7a (lynx)

This is the manifest for building IllusionX kernel for Pixel 7a (lynx)

## Syncing the source

```bash
# Create dir
mkdir -p ~/workdir
cd ~/workdir

# Init repo
repo init -u https://github.com/Blaster4385/kernel_manifest -b lynx

# Sync
repo sync -j$(nproc --all) --force-sync
```

## Building

```bash
LTO=full BUILD_AOSP_KERNEL=1 ./build_lynx.sh
```

## Submitting Patches

Patches are always welcome! Please submit your patches via a pull request to [Blaster4385/kernel_gs](https://github.com/Blaster4385/kernel_gs)

## Credits

* [Google](https://android.googlesource.com/kernel/common)
* [Panchajanya1999](https://github.com/Panchajanya1999/kernel-5.10)