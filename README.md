## Assign Keyboard Shortcut to ANY Menu Item in the Menu Bar

- `System Settings` >> `Keyboard` >> `Keyboard Shortcuts` >> `App Shortcuts` >> `+`

<img width="90" alt="Screenshot 2024-10-31 at 18 11 42" src="https://github.com/user-attachments/assets/8c3c8aeb-c669-42c0-8968-3fd535443a07">&nbsp;>>
<img width="200" alt="Screenshot 2024-10-31 at 18 12 27" src="https://github.com/user-attachments/assets/71c286aa-c41e-4849-9372-eddb6de5d37e">&nbsp;>>
<img width="80" alt="Screenshot 2024-10-31 at 18 12 52" src="https://github.com/user-attachments/assets/14efda50-79ff-4d5d-a4d5-aa02611f1bf5">&nbsp;>>
<img width="200" alt="Screenshot 2024-11-03 at 17 44 48" src="https://github.com/user-attachments/assets/e83c70ff-e9c1-44d7-8d93-75478f9cdcf1">&nbsp;>>
<img width="230" alt="Screenshot 2024-11-03 at 18 07 25" src="https://github.com/user-attachments/assets/1a3fbaf8-bbb0-4c1a-885a-f249ce562b1a">

- In `Menu Title`: Type the exact string seen (i.e. capital case, special characters, etc... must all correspond exactly) in the menu bar for your selected item.
- In `Keyboard Shortcut`: Click on the black box and type your desired shortcut

By default, this will apply to all applications. If you want it to apply only to a specific application, simply click on the `Application` picker and replace the choice "All Applications" with the one you desire.

### Open System Settings with `Cmd+Shift+,`

It is necessary to add the `...` as this is what is shown in the Menu Bar.

<img width="300" alt="Screenshot 2024-11-03 at 17 53 54" src="https://github.com/user-attachments/assets/c15b21c1-5763-4ac7-b823-9df56ee14a4b">

### Maximize Any Window with `Ctrl+F` (or `<other>`)

To go down a specific menu (to prevent selecting another menu item also called Zoom), we must use the keyword `->`.

If `Window->` is not specified to constrain the shortcut to the "Window" menu, this will try to find a `Zoom` menu item anywhere.

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

## Change Notification Sound

NO SOLUTION FOUND YET

##### Threads

https://apple.stackexchange.com/questions/302099/how-to-change-or-modify-the-macos-notifications-sound?answertab=scoredesc#tab-top
https://apple.stackexchange.com/questions/466822/how-to-change-default-notification-sound-tri-tone-for-all-apps-via-terminal
https://apple.stackexchange.com/questions/210072/where-are-the-alert-tone-audio-files-located-in-os-x/210074#210074

## Have more than 1 external screen

NO SOLUTION FOUND YET
