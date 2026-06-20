# OS Repository

https://github.com/secluso/os

https://www.yoctoproject.org
- Layers
- Recipes

https://github.com/siemens/kas
- pi-debug-image.yml
- pi-official-image.yml

https://docs.kernel.org/filesystems/squashfs.html

Partition layout: wic/sdcard-raspberrypi.wks
- https://docs.yoctoproject.org/ref-manual/kickstart.html

Reproducibility Changes:
- https://github.com/secluso/os/blob/main/meta-secluso-os/scripts/lib/wic/plugins/source/secluso_bootimg_partition.py
- https://github.com/secluso/os/blob/main/meta-secluso-os/recipes-multimedia/libcamera/0002-libcamera-make-dirty-version-suffix-reproducible.patch
- https://github.com/secluso/os/blob/main/meta-secluso-os/recipes-support/nss/nss_3.117.bbappend
- https://github.com/secluso/os/blob/main/meta-secluso-os/recipes-camera/libpisp/files/0001-src-meson-drop-build_rpath.patch
- 