Project Kaleidoscope
====================

Getting started
---------------

To get started with Kaleidoscope, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

To initialize your local repository, use this command:
```
repo init --no-clone-bundle -u https://github.com/Project-Kaleidoscope/android_manifest.git -b sunflower
```

Then to sync up:
```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune
```

Building
--------

Initialize the ROM environment with the envsetup.sh script.
```bash
. build/envsetup.sh
```

To lunch your device after cloning all device sources.
```bash
lunch kscope_<codename>-<buildtype>
```

Then start building.
```bash
mka bacon -j$(nproc --all)
```
