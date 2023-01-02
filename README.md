![NervaOS](https://github.com/NervaOS/manifest/blob/master/banner.png?raw=true)
# Getting started with NervaOS
a android based on AOSP


## Initialize Local Repository
-------------
```bash
repo init -u https://github.com/NervaOS/manifest -b $branch
```


## Syncing Repository
-------------
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```


## Lunch Command
-------------
```bash
. build/envsetup.sh
lunch nerva_$devicecodename-userdebug
make nerva -j$(nproc --all)
```


## Credits
 * [**AOSP**](https://android.googlesource.com)
