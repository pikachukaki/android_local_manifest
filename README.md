Local manifests for building CyanogenMod 10.1 for Huawei Device

How to build:
-------------

Initialize repo:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-10.1
    curl -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.github.com/pikachukaki/android_local_manifest/cm-10.1/local_manifest.xml
    repo sync

Compile:

    . build/envsetup.sh && brunch device_name
