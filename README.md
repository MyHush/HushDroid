# HushDroid

Hush Android Phone - Based on GrapheneOS

<img src="https://raw.githubusercontent.com/MyHush/HushDroid/master/hushdroid0.png">

## FAQ

### DIY install is cool, but how can I buy a fully setup HushDroid?

We are currently working on finalizing details and adding a shopping cart to our website so that HushDroids can be ordered
with BTC and HUSH and potentially a few others currencies.

The best way to stay informed is to join our [Discord](https://myhush.org/discord) in the #hushdroid channel, follow us on [Twitter](https://myhush.org/twitter), or follow us on [Mastodon](https://fosstodon.org/@myhushteam).

### Can I buy any random Android and install this?

No. Only Pixel 2 (legacy), Pixel 2 XL (legacy), Pixel 3, Pixel 3 XL, Pixel 3a, Pixel 3a XL, Pixel 4 and Pixel 4 XL will currently work, because that is all that [Graphene supports](https://grapheneos.org/faq).

### Can you support my random old Android phone?

No, please do not ask us. But you can use [LineageOS](https://lineageos.org) with SDA on any old phone for better privacy+security than old insecure stock Android. If you're unable to find an Official LineageOS build for your phone, then try searching [XDA Developers Forum](https://forum.xda-developers.com) to see if there is a current Unofficial LineageOS build for your phone.

### Will any Pixel 3 work?

No! It must be carrier-unlocked, so don't buy it from a carrier! This means do not buy it from Verizon or any phone carrier.
Buying directly from Google or Amazon or a third-party seller (like [Swappa](https://swappa.com)) is necessary but always check if it is carrier-unlocked before you but it. Phone companies do not want you to get rid of
their custom spyware that they charge other companies to place in their custom Android version. Never trust a phone from a carrier.

### Who is this phone for?

This is for people who value their privacy, especially location privacy. By avoiding a SIM and avoiding all Google services,
you have a much higher base level of privacy. This phone can be used for any purposes and is not special to Hush, other
than have Hush and Hush-vetted apps pre-installed with our custom default OS configuration.

### Should I do it myself or trust y'all?

If you have Linux CLI experience, you are able to do it all yourself and we highly recommend that. We do not want you to trust us unless you have to! For those that do not have Linux CLI experience, and who already trust Hush open source software, we feel this is a viable option which still greatly improves privacy.

Again, we prefer if you buy a Pixel yourself and do it all yourself, so you don't have to trust us with your hardware!
We know that is not an option for many people, so selling pre-installed HushDroids fills that gap.

### Does this replace my everyday phone?

No. This phone is a new, more private, isolated and compartmentalized device. You should avoid putting a SIM in it
to increase your location privacy and you shoud avoid installing various common apps that track you. So consider the HushDroid a new addition to your privacy toolbox, not a replacement for the insecure phone you must have to interact with the rest of society.

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


