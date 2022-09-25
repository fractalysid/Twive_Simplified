# Twive Simplified
Based on [Twive](https://github.com/fractalysid/Twive-Layout). Read Twive README for more info.

This is still Twive, with 2^5 keys, 5 layers and only 2 keys on the thumb cluster.

ZMK config files for the [Lucy](https://github.com/fractalysid/Lucy-Keyboard) v0.2 keyboard.
I couldn't manage to make the github action workflow work so it must be manually compiled.
A sample bash script to compile the firmware is provided, compile_example.sh. Remember to edit it modifying the variables.

[Here](https://github.com/fractalysid/qmk_firmware) you can find my fork of [QMK](https://github.com/qmk/qmk_firmware) with the layout for the ferris sweep (it is a modified version where the keys in the right half are in reverse order). You can also find the keymap.json in the QMK directory.

## Design principles differences with Twive
- Less layers, accessed through the thumb cluster
- A few combos to access extra keys which did not fit


### Details about layers and modifiers triggering
- Modifiers: Positional hold-tap, "tap-preferred" with 175ms tapping term
- Utility layer: default layer-toggle timings
- Common layer: "Balanced" with only 135ms tapping term for quick access while typing text

![Twive Simplified Layout](https://github.com/fractalysid/Twive_Simplified/blob/master/Twive.png?raw=true)
