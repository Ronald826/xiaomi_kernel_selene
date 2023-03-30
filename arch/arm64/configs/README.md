================================= Device Defconfig Guide ===================================

Defconfigs are crucial presets that are tailored to the device target.
Some defconfigs in here are designed for Generic desktops, Emulators and etc.

After selecting and compiling your desired defconfig, you can then proceed
customizing different configurations that your device supports.

In this folder we have 2 defconfigs that we use for the device Selene:

1. "selene_defconfig"   - Stock defconfig obtained not from MiCode Kernel Repo nor
                        from the other sources but, from the config.gz obtained 
                        from a running device in the directory /proc/config.gz.

2. "cselene_defconfig"  - A *Custom* defconfig for selene that is tailored by
                         d0g_kernel for your device. Majority of the changes from
                         Changelog is tweaked in here. MTK features that are disa-
                         bled from the stock_defconfig are enabled in this config

-

3. "selene.bak"         - Should not be really used. Most of the features here are
                          stripped and likely from the MiCode Repository. Features
                          like MTK Load Tracking in User and Kernel Space, MTK
                          SLBC, etc. are disabled. Not to mention, some of the stock 
                          defconfig features here are disabled This is a config that
                          was named, "selene_defconfig".