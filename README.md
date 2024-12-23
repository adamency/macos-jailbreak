## Assign Keyboard Shortcut to ANY Menu Item in the Menu Bar

As graphical programs on macos are restricted to a standard menu bar API, it is possible to assign a keyboard shortcut for any action in the menu bar for any given app or even all applications (provided the app provides the menu item in question in its menu bar).

The place to add shortcuts is there:

- `System Settings` >> `Keyboard` >> `Keyboard Shortcuts` >> `App Shortcuts` >> `+`

<img width="90" alt="Screenshot 2024-10-31 at 18 11 42" src="https://github.com/user-attachments/assets/8c3c8aeb-c669-42c0-8968-3fd535443a07">&nbsp;>>
<img width="200" alt="Screenshot 2024-10-31 at 18 12 27" src="https://github.com/user-attachments/assets/71c286aa-c41e-4849-9372-eddb6de5d37e">&nbsp;>>
<img width="80" alt="Screenshot 2024-10-31 at 18 12 52" src="https://github.com/user-attachments/assets/14efda50-79ff-4d5d-a4d5-aa02611f1bf5">&nbsp;>>
<img width="200" alt="Screenshot 2024-11-03 at 17 44 48" src="https://github.com/user-attachments/assets/e83c70ff-e9c1-44d7-8d93-75478f9cdcf1">&nbsp;>>
<img width="230" alt="Screenshot 2024-11-03 at 18 07 25" src="https://github.com/user-attachments/assets/1a3fbaf8-bbb0-4c1a-885a-f249ce562b1a">

- In `Menu Title`: Type the exact string seen (i.e. capital case, special characters, etc... must all correspond exactly) in the menu bar for your selected item.
- In `Keyboard Shortcut`: Click on the black box and type your desired shortcut

*NB: To go down a specific menu in the menu bar, we must use the keyword `->`. I.e. if we want to target the menu item `Close Tab` under the menu `File`, the "Menu Title" should be `File->Close Tab`.*

By default, this will apply to all applications. If you want it to apply only to a specific application, simply click on the `Application` picker and replace the choice "All Applications" with the one you desire.

### Examples

#### Open System Settings with `Cmd+Shift+,`

The System Settings is actually a menu item present for every app on the apple icon, which thus allows us to open it via a keyboard shortcut no matter which app is currently focused.

**Menu Item Path: `System Settings...`**

It is necessary to add the `...` as this is what is shown in the Menu Bar.

<img width="300" alt="Screenshot 2024-11-03 at 17 53 54" src="https://github.com/user-attachments/assets/c15b21c1-5763-4ac7-b823-9df56ee14a4b">

#### Maximize Any Window with `Ctrl+F` (or `<other>`)

The menu item action to maximize a window is called `Zoom` on macos. It is found in the `Window` menu.

**Menu Item Path: `Window->Zoom`**

If `Window->` is not specified to constrain the shortcut to the "Window" menu, this will try to find a `Zoom` menu item anywhere (which can happen).

<img width="300" alt="Screenshot 2024-11-03 at 17 53 30" src="https://github.com/user-attachments/assets/3eed3431-47bf-4537-927a-784eedaa3be0">


## Whitelist/Allow Any Unverified Program

1. Whitelist the binary for next run

```
spctl --add <myprogram>
```

2. Now run program

3. The system will still prevent its launch, but now you will be able to choose "Open"

4.  The program can now be opened/run without any restriction

[source1](https://github.molgen.mpg.de/pages/bs/macOSnotes/mac/mac_procs_unsigned.html)

## Desynchronize mouse/trackpad Scrolling Direction (use normal scrolling paradigm)

- Install Mos: https://github.com/Caldis/Mos/blob/master/README.enUS.md (main readme is in chinese)
- Run Mos
- Go to `Preferences` >> `General` >> `Scroll` >> Enable `Reverse Scroll`
- Add to `Open at Login` apps to persist across system restarts.

<img width="300" alt="Screenshot 2024-11-03 at 18 14 47" src="https://github.com/user-attachments/assets/5e612195-e28e-4257-b1b7-9f2555b55da6">

## Set separate Audio Output per Application

***No open-source solution found yet***

Some open-source projects for audio input/output manipulation on macos exist but none seem to allow using different audio outputs for different apps:

#### [BlackHole](https://github.com/ExistentialAudio/BlackHole)

Mainly for inter-app audio input/output management: e.g. redirecting audio output from apps as audio input to other apps.

But doesn't currently support redirecting app audio outputs to different audio output device/sink (<=> "sound output" in macos terminology)

[Related Issue](https://github.com/ExistentialAudio/BlackHole/discussions/40)

#### [BackgroundMusic](https://github.com/kyleneideck/BackgroundMusic)

Provides separate volume setting per app, but again no separate audio output device.

[Related Issue](https://github.com/kyleneideck/BackgroundMusic/issues/661)

#### [Proxy Audio Device](https://github.com/briankendall/proxy-audio-device)

TODO

## Have more than 1 external screen

Macbook Airs are artificially limited to 1 external monitor.

***No open-source solution found yet***

It is possible to overcome this limitation via a software middleman technology called DisplayLink.

It however needs a hardware component alongside it to work: a DisplayLink-supported USB hub.

The idea is that the hub will convert the hardware output to a digital input that will then be sent/received to/from the laptop into the DisplayLink software that will then interface with the OS to make it think it has two physical monitors plugged and bypassing the CPU limitation. (need better explanation)

## Change Notification Sound

NO SOLUTION FOUND YET

##### Threads

https://apple.stackexchange.com/questions/302099/how-to-change-or-modify-the-macos-notifications-sound?answertab=scoredesc#tab-top
https://apple.stackexchange.com/questions/466822/how-to-change-default-notification-sound-tri-tone-for-all-apps-via-terminal
https://apple.stackexchange.com/questions/210072/where-are-the-alert-tone-audio-files-located-in-os-x/210074#210074

