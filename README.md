Android Platform Manifest

- **Get the source:**

        $ mkdir THUNDERKAT
        $ cd THUNDERKAT
        $ repo init -u https://github.com/craigacgomez/platform_manifest -b thunderkat
        $ repo sync

- **Update the source:**

        $ cd THUNDERKAT
        $ repo sync

- **Building**

        $ source build/envsetup.sh
        $ lunch aosp_<device>-userdebug (e.g. aosp_manta-userdebug)
        $ make -j `getconf _NPROCESSORS_ONLN` otapackage

- **Cleaning**

        $ source build/envsetup.sh
        $ make clean
