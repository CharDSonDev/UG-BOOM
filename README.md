# UG-BOOM

It only works by turning off

![Screenshot from 2023-01-30 17-19-32](https://user-images.githubusercontent.com/36754778/215602870-49415ebc-2af0-4260-822a-806b603ffdfe.png)

## gatttool comands:

Power On:
```console
gatttool -i hci0 -b **UE BOOM MAC** --char-write-req -a 0x0003 -n **DEVICE MAC with ':'**01
```

Power Off:
```console
gatttool -i hci0 -b **UE BOOM MAC** --char-write-req -a 0x0003 -n **DEVICE MAC with ':'**02
```

UE BOOM Name:
```console
gatttool -i hci0 -b **UE BOOM MAC** --char-read --uuid 0x2a00
```

UE BOOM Battery Level
```console
gatttool -i hci0 -b **UE BOOM MAC** --char-read --uuid 0x2a19
````

## More information about how to control UE BOOM loudspeakers from Linux and macOS:
* Android APP: https://github.com/Shingyx/BoomSwitch
* NPM Plugin: https://github.com/alessandroaime/homebridge-ueboom
* gatttool commands: https://gist.github.com/marcust/af93ff47899583f5a52f
* Python console: https://github.com/eni23/ueboom
* UE BOOM APP Source: https://www.reddit.com/r/bluetooth/comments/ap6npx/bluetooth_protocol_for_ue_boom_2/
* gatttool details: https://github.com/kancelott/ue-boom-2-bt-le-reverse-engineering
* MacOS Shortcuts: https://www.reddit.com/r/shortcuts/comments/dz9zun/finally_turn_on_ue_boom_bluetooth_speaker/
* Blueman plugin: https://github.com/edgarogh/blueman-ueboom
* Swift APP: https://github.com/smpanaro/ue-speaker-app
* gatttool docs: http://tvaira.free.fr/flower-power/gatttool.txt
* gatttool char write: https://stackoverflow.com/questions/58814890/gatttool-non-interactive-mode-multiple-char-write-req
* more: https://gist.github.com/LieBtrau/e98b0e796c6d2990007f1d5cbe7675fe
* Bluetooth UIDD: https://www.bluetooth.com/specifications/assigned-numbers/
* GitHub other console app: https://github.com/Samt43/HackBOOM2
* X2: https://github.com/Felix-Pi/UE_BOOM_controller
