## OPLUS-QQCandy-Dev - Personal extras

This organization contains repositories to build AOSP / LineageOS 24 ROMs for
**OnePlus Ace Racing Edition (PGZ110)** and **OPPO K10 (PGJM10)** on the
MediaTek MT6895 `qqcandy` platform.

This is a single-SKU project: both devices run the same image and are presented
as **OnePlus Ace Racing Edition**. The 21143 and 22801 camera paths are both
kept.

* [**Device Tree (common)**](https://github.com/OPLUS-QQCandy-Dev/android_device_oplus_mt6895-common.git) (`android_device_oplus_mt6895-common`)
* [**Vendor Tree (common)**](https://github.com/OPLUS-QQCandy-Dev/android_vendor_oplus_mt6895-common.git) (`android_vendor_oplus_mt6895-common`)
* [**Prebuilt Kernel**](https://github.com/OPLUS-QQCandy-Dev/android_device_oplus_mt6895-kernel.git) (`android_device_oplus_mt6895-kernel`)

### OnePlus Ace Racing Edition (PGZ110)
<img width="260" src="https://raw.githubusercontent.com/OPLUS-QQCandy-Dev/.github/lineage-24.0/profile/ace-racing.png?v=2" alt="OnePlus Ace Racing Edition">

### OPPO K10 (PGJM10)
<img width="260" src="https://raw.githubusercontent.com/OPLUS-QQCandy-Dev/.github/lineage-24.0/profile/oppo-k10.png" alt="OPPO K10">


* [**Device Tree (qqcandy)**](https://github.com/OPLUS-QQCandy-Dev/android_device_oplus_qqcandy.git) (`android_device_oplus_qqcandy`)
* [**Vendor Tree (qqcandy)**](https://github.com/OPLUS-QQCandy-Dev/android_vendor_oplus_qqcandy.git) (`android_vendor_oplus_qqcandy`)

### Other required repositories
* [**Mediatek Sepolicy**](https://github.com/LineageOS/android_device_mediatek_sepolicy_vndr.git) (`android_device_mediatek_sepolicy_vndr`)
* [**Mediatek Hardware**](https://github.com/LineageOS/android_hardware_mediatek.git) (`android_hardware_mediatek`)
* [**OPLUS Hardware**](https://github.com/LineageOS/android_hardware_oplus.git) (`android_hardware_oplus`)
* [**Lineage Interfaces**](https://github.com/LineageOS/android_hardware_lineage_interfaces.git) (`android_hardware_lineage_interfaces`)
* [**Lineage Sepolicy**](https://github.com/LineageOS/android_device_lineage_sepolicy.git) (`android_device_lineage_sepolicy`)
* [**Google Pixel Hardware**](https://github.com/LineageOS/android_hardware_google_pixel.git) (`android_hardware_google_pixel`)

### Build
```bash
lunch lineage_qqcandy-userdebug
mka bacon -j$(nproc)
```

Expanded `super` only:

```bash
QQCANDY_EXPANDED_SUPER=true mka bacon -j$(nproc)
```
