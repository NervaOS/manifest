Getting started with NervaOS

====================

![NervaOS](https://github.com/NervaOS/manifest/blob/master/banner.png?raw=true)

Initialize Local Repository

-------------

```bash

  repo init -u https://github.com/NervaOS/manifest -b <select_branch>

```

Syncing Repository

-------------

```bash

   repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

```

Lunch Command

-------------

```bash

  . build/envsetup.sh
  lunch nerva_<devicecodename>-userdebug
  mka bacon -j$(nproc --all)
```





