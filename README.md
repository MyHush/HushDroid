# HushDroid

Hush Android Phone - Based on GrapheneOS

## How to Install Your own HushDroid

Firstly, we will be installing GrapheneOS.



## Things You Will Need
  * wifi access (to give to the phone)
  * USB cable to connect phone to computer
  
  

  * Read https://grapheneos.org/install
  * Install the correct version of `fastboot` from https://developer.android.com/studio/releases/platform-tools , must have at least 28.0.2 . Installing the latest version is probably best
  * `fastboot --version` to see installed version
  
  ```
  sudo fastboot flashing unlock
  # download appropriate file for your phone hardware
  unzip xxx
  cd xxx
  sudo ./flash-all.sh
  ```
  
  
