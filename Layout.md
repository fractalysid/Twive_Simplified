# To-Be-Named-Yet Layout
Inspired by pierrechevalier83 [layout](https://github.com/qmk/qmk_firmware/tree/master/keyboards/ferris/keymaps/default) for ferris.

This will have it's own repository one day.

- Colemak-DH as base layer
- Space on right thumb, Return on left one
- Apostrophe on bottom pinky. Very common in italian language. Swap with another common symbol or letter
- Backspace always accessible from top pinky
- Modifiers on bottom row, mirrored. From left to right: SHIFT, CTRL, ALT, GUI
- Layers on home row
- "Utility" layer on right thumb for keys like GUI, TAB, ESC, sticky modifiers and more
- "Common" layer on left thumb for common letters and symbols used in various languages. Useful for accented letters and other language specific symbols. Also useful for commonly used symbols (I'm currently using it for bash symbols)
- "Utility" layer on right thumb for TAB, ESC, GUI, sticky modifiers and so on
- No use of SHIFT for symbols
- No use of combos (almost)

More details:
- Home row layer toggle: Positional hold-tap, "tap-preferred" with 250ms tapping term. 220 should be feasible for most
- Bottom row modifier: Positional hold-tap, "tap-preferred" with 200ms tapping term
- Common layer: default layer-toggle timings
- Utility layer: Balanced with only 150ms tapping term for quick access while typing text

# Layers
There are 10 layers:
- BASE: Colemak-DH
- UTILITY
- COMMON
- RIGHT SYMBOLS
- LEFT SYMBOLS
- FUNCTIONS
- NUMBERS
- MEDIA
- KEYBOARD
- QWERTY

Layers in the home row are placed in order to have the most used ones in the inner
and outer fingers balanced between left and right ( not considering pinkies in this case).
This is in order to balance usage of the hands and minimize confusion when in need of quickly
switching between layers (eg: round parentheses and navigation to move inside )

|  NUMBERS  |  MEDIA   | RSYMBOLS  |       | LSYMBOLS  | FUNCTIONS | NAVIGATION |
|:---------:|:--------:|:---------:|:-----:|:---------:|:---------:|:----------:|
| High Freq | Low Freq | High Freq |       | High Freq | Low Freq  | High Freq  |

## Base
Here we find the COLEMAK-DH. Hyphen is replaced by Apostrophe ' as it is very common
in the italian language. Replace it with a commonly used symbol of your liking.
In the top pinky we find the "backspace" which is always accessible from every layer
except the UTILITY layer, which replaces it with "delete" and the COMMON layer, which
sends CTRL+backspace in order to delete entire words.
It is also not accessible from the KEYBOARD and QWERTY layouts.

## Utility
This layer is for utility. We have LGUI in the home index finger. TAB and ESC are
placed similar to a standard keyboard but using the home row or just the left index
finger is a good idea.
This layer can be thought as the layer in which to place all the utility keys, like
return, esc, backspace, delete... and even remove them from the base layer and thumb
cluster.
Here we can also place other utility keys like PRINTSCREEN, INSERT and so on.
I'm experimenting with copy-cut-paste in the right home row right now. Comfortable
but could be better.
In the left home row you can find sticky modifiers. I found very comfortable to
use sticky modifiers in this layer for actions like "save" (Ctrl + S), "quit" (Ctrl + Q),
"open terminal" (Ctrl + Alt + T), by pressing keys in sequence and avoid the use
of combos.
Also present is the caps-word feature, which I found extremely useful.

## Common
This layer is accessed with a very short timing, which you probably want to
tune to your typing speed and style. It's goal is to be the home for all those
letters and symbols commonly used while writing normal text. This will be
particularly useful for all european languages with a lot of extra letters.
Right now I'm using it for accented letters, question and exclamation mark, hyphen,
underscore and other symbols frequently used in bash.

Backspace is replaced by CTRL + Backspace.

## Navigation
Vim style navigation right now but I am considering the WASD style.
Access to home, end, page up, page down, tab left and tab right (to move between tabs
in the browser), alt-tab window navigation, previous, next, upper workspace, lower workspace.
Modifiers are accessible but also added for convenience.
This will probably be reworked when mouse emulation will be merged in the main 
zmk repository.

## Right symbols
Common parentheses in home row. Brackets and angular in top row. Other common
programming symbols in bottom row.
Bottom row for rare symbols.

## Left symbols
Common symbols in home row. Math symbols in home row.
Bottom row for rare symbols.

## Function
F1-F12. Other special functions may be added.

## Numbers
Rolling hands from outer to inner side is more comfortable. Moreover 0123 are
more common than other numbers. Keys are placed keeping these things in mind.
Dot and comma and a couple of math operators are also present.

## Media
Play/Pause, Previous, Next, Stop on home row.
Volume top left. Brightness top right.
Free bottom row.

## Keyboard
This is accessed Functions related to keyboard. Reset, bootloader mode, bluetooth profile management,
RGBs and so on.

From here you can also activate the QWERTY layer.

## Qwerty
QWERTY layer with backspace in the right home pinky.

Press both thumb keys to get back to BASE layer.