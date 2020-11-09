TWRP Device Tree for Xiaomi Redmi Go
====================================

## Features

This TWRP automatically detects the device region and updates the device code name _"tiare"_

## Compile

First checkout Minimal TWRP with OmniROM Tree:

```
repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0
repo sync
```

And execute these:

```
export ALLOW_MISSING_DEPENDENCIES=true # Only if using Minimal TWRP Tree
. build/envsetup.sh
lunch omni_tiare-eng
mka recoveryimage
```

## Installing:

Testing it:
```
fastboot boot out/target/product/tiare/recovery.img
```

Flash it via fastboot:
```
fastboot flash recovery recovery.img
```

Or use Official TWRP App to install it.

## Credits

Thanks to @mauronofrio for his work on TWRP

Thanks to @Dhina_17 for 'onclite' blobs
