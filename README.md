## TWRP device tree for Huawei Honor 3C Lite (holly)

Add to `.repo/local_manifests/holly.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/huawei/holly" name="android_device_huawei_holly" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_holly-eng
make -j5 recoveryimage
```
