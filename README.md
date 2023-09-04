# Red-Magic-6S-Pro-China-Update

## Step to root

Need unlock bootloader first.

```sh
adb reboot fastboot
fastboot flash boot PATH_TO_BOOT_FILE
fastboot reboot
```

## Full update packages

You should flash and update to version 8.20 before flashing magisk patched boot.
[Download v8.12](http://romdownload.nubia.com/%E7%BA%A2%E9%AD%946S%20Pro/V8.12/NX669S-update.zip)

## Unlock all google feature (make it works like global version)

Flash these modules in magisk (delta). And remember to grant all permission in assistant, google, android auto, google play service, google play store, google service framework. (depend on your phone, chose the right android version)

### Update google play service

https://play.google.com/store/apps/details?id=com.google.android.gms&hl=en&gl=US

### fix google contacts, calendar not sync and lost google play store icon:

Install google play store, google contacts sync, google calendar sync from apk files (get from apkmirror,  etc.).

### fix android wear os gsm version and google location:

https://github.com/fei-ke/unlock-cn-gms/releases

### fix android auto

After flash this module, search bar in setting to find "android auto". 
https://github.com/AndroPlus-org/magisk-module-androidauto/releases

### fix anhroid assistant (enable hello google and lockscreen hellogoogle)

https://github.com/AndroPlus-org/magisk-module-assistant/releases

### fix delay notifications

1. go to setting > apps > self-start manage > check all the app you need to receive notifications in the background (eg: fb, reddit, x, etc)
2. go to setting > notification and status bar > notification management > switch to third-party apps tab > open all the apps you want to receive notifications.
3. go to setting > power management > application power management > click on the app and select "regardless of control" for the same app from step 1 2. (gg assistant, calendar/contacts sync, 
gmail, or any apps that play music in background while screen is locked should be selected)
