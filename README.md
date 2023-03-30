## Repo Init ##
```bash
repo init -u https://github.com/neilchetty/android_kernel_manifest.git -b android-mtk-rmx3031-4.19-android11
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```
## Building Kernel ##
```bash
BUILD_CONFIG=kernel/realme/RMX3031/build.config.cupida build/build.sh
```

