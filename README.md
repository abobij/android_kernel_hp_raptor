# HP Pro x3 kernel

Linux 3.18.31 port for the HP Pro x3 (raptor, MSM8996), based on CAF `LA.UM.5.5.r1-04900-8x96.0`.

## Tested on the RAPTOR test build

- Boots stock Android 7.1.2 with the RAPTOR device tree.
- Display, touchscreen, brightness control, hardware buttons, vibration, and USB ADB.
- Wi-Fi with a matching signed QCACLD 2.0 module in the boot ramdisk.
- Bluetooth pairing/connectivity.
- Thermal sensors, auto-rotate, light/proximity sensors.

## Known issues and incomplete support

- Camera/Flash and NFC are disabled while the board wiring is being ported.
- Bootanimation and lockscreen can finish loading slowly.
- Sometimes apps open slowly. App opening animation from Recents is laggy.
- No sound from speakers at all
- Sound menu in settings hangs the app if the Bluetooth headset is connected. Needs testing.
- Wake from suspend has a latency after pressing the power button.
- No fingerprint support.

## Untested

- Audio recording, offline/online charging, doze, DP Alt Mode.
- Cellular calls and data - modem will never be tested fully by me due to lack of a physical sim-card.
- HW Video decoding, CPU/GPU Frequency scaling, Vulkan/OpenGLES, governors, fuel gauge.

See [COPYING](COPYING) for licensing information.
