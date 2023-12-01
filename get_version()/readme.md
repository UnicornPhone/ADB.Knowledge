get_version() https://www.google.com/search?q=adb+get+android+version https://stackoverflow.com/questions/29968096/get-android-os-version-of-device-connected-via-adb

https://medium.com/@theapache64/adb-say-bye-to-multi-device-error-240ba10777a2

```
adb devices
dev="localhost:5555"

adb -s $dev shell getprop ro.build.version.release
adb -s $dev shell getprop ro.build.version.sdk
```
