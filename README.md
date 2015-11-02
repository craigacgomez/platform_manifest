Android Platform Manifest - Marshmallicious

- **Get the source:**

        $ mkdir MARSHMALLICIOUS
        $ cd MARSHMALLICIOUS
        $ repo init -u https://github.com/craigacgomez/platform_manifest -b marshmallicious
        $ repo sync

- **Update the source:**

        $ cd MARSHMALLICIOUS
        $ repo sync

- **Building**

        $ source build/envsetup.sh
        $ lunch aosp_<device>-userdebug (e.g. aosp_flounder-userdebug)
        $ make -j `getconf _NPROCESSORS_ONLN` otapackage

- **Cleaning**

        $ source build/envsetup.sh
        $ make clean
