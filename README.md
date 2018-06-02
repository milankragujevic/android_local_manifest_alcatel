# Alcatel POP 4 LineageOS local manifest

    repo init -u git://github.com/LineageOS/android.git -b cm-13.0
    curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.githubusercontent.com/milankragujevic/android_local_manifest_alcatel/cm-13.0/local_manifest_pop4.xml
    repo sync

---

    source ./build/envsetup.sh
    lunch cm_pop4-userdebug
    make otapackage
