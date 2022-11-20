# Enabling 32-bit support on the Pixel 7
Pixel 7 vendor build.prop files with 32-bit support

**Meant to be used in conjunction with $PLACEHOLDER**

The build.prop files are specifically the ones from `/vendor/build.prop`.

They have been pre-modified to allow for 32-bit support by enabling `Zygote64_32` and adding `armeabi-v7a` and `armeabi` to the ABI lists.

## Easy Download Links
- [Pixel 7 Pro - November 2022 - Global](https://raw.githubusercontent.com/Namelesswonder/pixel7_vendor_build_props/main/cheetah-td1a.221105.001/build.prop)
- [Pixel 7 Pro - November 2022 - Telia](https://raw.githubusercontent.com/Namelesswonder/pixel7_vendor_build_props/main/cheetah-td1a.221105.001.a1/build.prop)
- [Pixel 7 Pro - November 2022 - Verizon](https://raw.githubusercontent.com/Namelesswonder/pixel7_vendor_build_props/main/cheetah-td1a.221105.003/build.prop)
- [Pixel 7 Pro - November 2022 - QPR1 Beta 3.1](https://raw.githubusercontent.com/Namelesswonder/pixel7_vendor_build_props/main/cheetah-t1b3.221003.008/build.prop)
- [Pixel 7 - November 2022 - Global](https://raw.githubusercontent.com/Namelesswonder/pixel7_vendor_build_props/main/panther-td1a.221105.001/build.prop)
- [Pixel 7 - November 2022 - Telia](https://raw.githubusercontent.com/Namelesswonder/pixel7_vendor_build_props/main/panther-td1a.221105.001.a1/build.prop)
- [Pixel 7 - November 2022 - Verizon](https://raw.githubusercontent.com/Namelesswonder/pixel7_vendor_build_props/main/panther-td1a.221105.003/build.prop)
- [Pixel 7 - November 2022 - QPR1 Beta 3.1](https://raw.githubusercontent.com/Namelesswonder/pixel7_vendor_build_props/main/panther-t1b3.221003.008/build.prop)

## Folder structure for the repo
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

# Modifications
```
ro.zygote=zygote64_32
ro.vendor.product.cpu.abilist=arm64-v8a,armeabi-v7a,armeabi
ro.vendor.product.cpu.abilist32=armeabi-v7a,armeabi
```
