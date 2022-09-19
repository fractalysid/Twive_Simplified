# Twive Layout
Inspired by pierrechevalier83 [layout](https://github.com/qmk/qmk_firmware/tree/master/keyboards/ferris/keymaps/default) for ferris.

Graphic made with draw.io, thanks [Duccio](https://github.com/duckyb/zmk-sweep) for the idea!

I present to you: Twive!

The name comes from the contraption of the words "Two" and "Five". Why this name?
Well, because 2^5 keys, 2*5 layers ~~and LSD-25~~ is all you will ever need.


The basic ideas are set but I keep changing everything based on my use feedback.

ZMK config files for the [Lucy](https://github.com/fractalysid/Lucy-Keyboard) v0.2 keyboard.
I couldn't manage to make the github action workflow work so it must be manually compiled.

## Design principles:

- 32 keys (2^5) with only 1 key on the thumb cluster
- 10 layouts (2*5)
- Colemak-DH as base layer
- Space on right thumb, Return on left one
- Apostrophe on bottom pinky. Very common in italian language. Swap with another common symbol or letter
- Backspace always accessible from top pinky
- Modifiers on bottom row, mirrored. From left to right: SHIFT, CTRL, ALT, GUI
- Layers on home row
- "Utility" layer on right thumb for keys like GUI, TAB, ESC, sticky modifiers, macros and more
- "Common" layer on left thumb for common letters and symbols used in various languages. Useful for accented letters, other language specific symbols and commonly used symbols (I'm currently using it for bash symbols)
- "Utility" layer on right thumb for TAB, ESC, GUI, sticky modifiers and so on
- No use of SHIFT for symbols
- No use of combos (almost)
- Prefer more layers and avoid using keys in difficult positions (a few exceptions exist where I preferred keeping the standard position)
- An extra QWERTY layer in case someone else needs to use your keyboard or you want to game with it
- "Ok wait! you lied! we've got 11 layers!". I did not, Qwerty does not count as it is an extra layer for extremely rare use cases

### Details about layers and modifiers triggering
- Home row layer toggle: Positional hold-tap, "tap-preferred" with 200ms tapping term
- Bottom row modifier: Positional hold-tap, "tap-preferred" with 175ms tapping term
- Utility layer: default layer-toggle timings
- Common layer: "Balanced" with only 135ms tapping term for quick access while typing text

The idea behind the 
 thumb cluster keys is that we can afford such a low tapping term on the left one
because Return is not pressed inside a sentence like "space" so there is no risk of misfiring the layer toggle
when we didn't mean to while writing a sentence. While on the right one we mainly map utility keys so nothing
that needs to be used in a sentence.

# Layers
There are 10 layers:
- BASE: Colemak-DH
- UTILITY
- COMMON
- SYMBOLS 1
- SYMBOLS 2
- FUNCTIONS
- NUMBERS
- NAVIGATION
- MEDIA
- KEYBOARD
- ~~QWERTY~~

Idea for layer keys comes from the fact that simbols and numbers most probably requires the backspace
to be accessible while using to they are in the right side. All the others are on the left side so we
can use the right pinky key that is otherwise reserved for backspace.

## Base
Here we find the COLEMAK-DH. Hyphen is replaced by Apostrophe ' as it is very common
in the italian language. Replace it with a commonly used symbol of your liking.
In the top pinky we find the "backspace" which is always accessible from every layer
except the UTILITY layer, which replaces it with "delete" and the COMMON layer, which
sends CTRL+backspace in order to delete entire words.

## Utility
This layer is for utility. We have LGUI in the home index finger. TAB and ESC are
placed similar to a standard keyboard but it would be a good idea to place them
in the index finger column.
This layer can be thought as the layer in which to place all the utility keys, like
return, esc, backspace, delete... and even remove them from the base layer and thumb
cluster.
Here we can also place other utility keys like PRINTSCREEN, INSERT and so on.
I'm experimenting with copy-cut-paste in the right home row right now and undo-redo
in the top row. Comfortable but could be better.
In the left home row you can find sticky modifiers. I found very comfortable to
use sticky modifiers in this layer for actions like "save" (Ctrl + S), "quit" (Ctrl + Q),
"find" (Ctrl + f), "open terminal" (Ctrl + Alt + T), by pressing keys in sequenceand
avoid the use of combos.
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
'(){' becomes a matter of rolling the keys from inner to outer column. It couldn't be
easier.

## Left symbols
Common symbols in home row. Math symbols in top row.
Bottom row for rare symbols.

## Function
F1-F12. Other special functions may be added.
Ctrl+Alt for convenient access to terminal consoles in GNU/Linux.

## Numbers
0123 are more common than other numbers so they are in the home row.
Dot and comma and a couple of math operators are also present.

## Media
Play/Pause, Previous, Next, Stop on home row.
Volume top left. Brightness top right.
Free bottom row.

## Keyboard
This is to access functions related to keyboard. Reset, bootloader mode, bluetooth
profile management, usb over ble preference, RGBs and so on.

From here you can also activate the QWERTY layer.

## Qwerty
QWERTY layer with backspace in the right home pinky.
RET and SPC are swapped as SPACE is used in videogames.

Press both thumb keys to get back to BASE layer.

# Twive

![Twive Layout](https://github.com/fractalysid/Twive-Layout/blob/symbols_rework/Twive.png?raw=true)
