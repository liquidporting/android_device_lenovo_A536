## TWRP device tree for Lenovo A536 (A536)

Add to `.repo/local_manifests/A536.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/lenovo/A536" name="android_device_lenovo_A536" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_A536-eng
make -j5 recoveryimage
```
