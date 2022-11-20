# Enabling 32-bit support on the Pixel 7
Pixel 7 vendor build.prop files with 32-bit support

**Meant to be used in conjunction with $PLACEHOLDER**

Folder structure for the repo is:
```
  [Repo]
       \ 
        |- [Name-Release Version]
        |                  \
        |                   |- build.prop
        |          
        |- [Name-Release Version]
        |                  \
        |                   |- build.prop
        |
        ...
```

With `name` being the codename for your device and `release version` being what you are using.  
- Pixel 7 Pro - `cheetah`  
- Pixel 7 - `panther`

The build.prop files are specifically the ones from `/vendor/build.prop`.

They have been pre-modified to allow for 32-bit support by enabling `Zygote64_32` and adding `armeabi-v7a` and `armeabi` to the ABI lists.

# Modifications
```
ro.zygote=zygote64_32
ro.vendor.product.cpu.abilist=arm64-v8a,armeabi-v7a,armeabi
ro.vendor.product.cpu.abilist32=armeabi-v7a,armeabi
```
