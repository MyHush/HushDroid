# HushDroid

Hush Android Phone - Based on GrapheneOS

<img src="https://raw.githubusercontent.com/MyHush/HushDroid/master/hushdroid0.png">

## FAQ

### Can I buy any random Android and install this?

No. Only Pixel 3, Pixel 3a, Pixel 3 XL and Pixel 3a XL will currently work, because that is all that Graphene supports.

### Can you support my random old Android phone?

No, please do not ask us.

## Will any Pixel 3 work?

No! It must be carrier-unlocked, so don't buy it from a carrier! This means do not buy it from Verizon or any phone carrier.
Buying directly from Google or Amazon or a third-party seller is necessary. Phone companies do not want you to get rid of
their custom spyware that they charge other companies to place in their custom Android version. Never trust a phone from a carrier.

## How to Install Your own HushDroid

Firstly, we will be installing GrapheneOS. This "Tales From The Crypt" video shows every step in an easy-to-follow way:

https://www.youtube.com/watch?v=oO0UFZjuotg&feature=youtu.be





## Things You Will Need
  * wifi access (to give to the phone)
  * USB-C cable to connect phone to computer. Make sure to use the cable that came with the phone! Others are likely to not work correctly.
  * Read https://grapheneos.org/install
  * Install the correct version of `fastboot` from https://developer.android.com/studio/releases/platform-tools , must have at least 28.0.2 . Installing the latest version is probably best
  * `fastboot --version` to see installed version
  
## Boot into your bootloader

First hold down "Volume Down" then press the Power button for a few seconds.

<img src="https://raw.githubusercontent.com/MyHush/HushDroid/master/graphene0.png">

## Unlocked bootloader

  ```
  sudo fastboot flashing unlock
  ```

Once your bootloader is unlocked, it should look like this:

<img src="https://raw.githubusercontent.com/MyHush/HushDroid/master/graphene1.png">

With an unlocked bootloader, you are able to install any operating system you want! Freedom!
NOTE: Also remember, we must re-lock the bootloader when we are done, or somebody who steals your
phone can easily wipe all the data and install something new.


## Flash Graphene
  
  ```
  # download appropriate file for your phone hardware
  unzip xxx
  cd xxx
  sudo ./flash-all.sh
  ```
  
## Re-lock bootloader

```
sudo fastboot flashing lock
```

Now you have a phone which doesn't spy on you, as long as you don't put in a SIM or opt-in to Google services.

## Installing SDA app

Currently SDA is only on Google Play, but not yet on FDroid, so you will need to install from Github and enable the installing of "untrusted" APKs


<img src="https://raw.githubusercontent.com/MyHush/HushDroid/master/hushdroid1.png">

<img src="https://raw.githubusercontent.com/MyHush/HushDroid/master/hushdroid2.png">



  
  
