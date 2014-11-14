Android Platform Manifest - Lollipopalooza

- **Get the source:**

        $ mkdir LOLLIPOPALOOZA
        $ cd LOLLIPOPALOOZA
        $ repo init -u https://github.com/craigacgomez/platform_manifest -b lollipopalooza
        $ repo sync

- **Update the source:**

        $ cd LOLLIPOPALOOZA
        $ repo sync

- **Building**

        $ source build/envsetup.sh
        $ lunch aosp_<device>-userdebug (e.g. aosp_manta-userdebug/aosp_flounder-userdebug)
        $ make -j `getconf _NPROCESSORS_ONLN` otapackage

- **Cleaning**

        $ source build/envsetup.sh
        $ make clean
