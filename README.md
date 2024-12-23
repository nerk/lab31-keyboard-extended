# Lab31 German Keyboard Extended Layout

This is an Android application to provide an additional keyboard layout for the German
version (QWERTZ) of the foldable Lab31 Bluetooth keyboard.

[This keyboard](https://www.action.com/de-de/p/3203226/lab31-faltbare-drahtlose-tastatur/)
is being sold at local Action stores in Germany for only € 6.95.

The quality is actually pretty decent for its extremely low price.

Unfortunately, the keyboard layout of the German version is almost unusable, if you
want to use the keyboard as a developer. The pipe symbol is not mapped to any
key, there is no way to enter it from the keyboard. ESC key and  < > characters can only be accessed in
combination with the FN key. All other special characters can be accessed as
usual as with any QWERTZ layout, although they are not printed on the keycaps.

By installing this application, the layout is modified as follows:

* The left command key is mapped to the combined <>| key as found on QWERTZ
  keyboards. Pressing this key without any modifier yields <, using Shift+
  left command yields >, AltGr+left command yields |.
* The CapsLock key is mapped to ESC.

Download the latest zip file from [Releases](https://github.com/nerk/lab31-keyboard-extended/releases), 
unzip the contents. Install the apk file on your Android device, connect your Lab31 keyboard via Bluetooth and
select "Lab31 German (DE), Dev" from the list of keyboard layouts for the physical keyboard in device settings.
This app does not provide any UI and does not require root access to your
device.


This application is based on [this](https://github.com/ris58h/custom-keyboard-layout) skeleton project. 

# Building
Clone the project

Build with 

```
./gradlew build
```


The ready-to-install apk-file can be found at
```
./app/build/outputs/apk/release
```

Install the apk and select the Lab31 layout in device settings.
