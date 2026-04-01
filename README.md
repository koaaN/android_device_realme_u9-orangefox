# Realme NEO8 u9 OrangeFox device tree

# How To Build

### Clone & Sync Source
```
mkdir -p ~/android/OrangeFox_14
cd ~/android/OrangeFox_14
git clone https://gitlab.com/OrangeFox/sync.git
cd sync
./orangefox_sync.sh --branch 14.1 --path ~/android/fox_14.1
```
### Clone Device-tree
```
cd ~/android/fox_14.1/device
mkdir -p realme
cd oneplus
git clone https://github.com/koaaN/android_device_realme_u9-orangefox u9
```
### BUILD!
```
cd ~/android/fox_14.1
source build/envsetup.sh
lunch twrp_u9-ap2a-eng
mka adbd recoveryimage
```
