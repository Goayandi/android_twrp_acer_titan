Acer Iconia Tab A3-A50 (titan, acer_Titan)
===============
```
By : Goayandi
```
![Iconia Tab A3-A50](https://www.notebookcheck.com/fileadmin/Notebooks/Acer/Iconia_Tab_10_A3-A50/acer_iconia_tab_10_a3_a50_android_wp_03_59a6b83ee9aa5.jpg)

The Acer Iconia Tab A3-A50 (codename _"titan / acer_Titan"_) is a tablet from Acer.

This is a Minimal Device Tree for building TWRP for Iconia Tab A3-A50. I used TWRP by multirom and TWRP for Asus Zenpad 3S 10 from rakomancha to finally build a working tree for Mi Pad 3 and now ported it to Iconia Tab A3-A50.

Basic        | Spec Sheet
------------:|:------------------------
CPU          | Cortex-A72 & Cortex-A53 | Hexa-Core | MT8176
GPU          | PowerVR GX6250
Memory       | 4GB RAM
Shipped Android Version | 7.0
Storage      | 64GB
Battery      | 6100 mAh Li-Po
Display      | 10.1
Rear Camera  | 5.0 MP , Video
Front Camera | 2.0 MP


This branch is for building TWRP.

### Thanks to:
 * Team M.A.D
 * rakomancha

### To build: 
```

$ repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

To initialize a shallow clone, which will save even more space, use a command like this:

$ repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

After that sync your sources:

$ repo sync

Build your recovery:

$ source build/envsetup.sh

& lunch acer_Titan-eng

make clean && make recoveryimage
```
