# rain toe

## Acknowledgements
This started with Ardux [https://ardux.io/] and with The Paintbrush [https://github.com/artseyio/thepaintbrush] ... both are amazing! Thank you KemoNine :) 

## Design aims
* This is intended to just be an 8 key layout; not extended.
* It's primarily left-handed. Might make a right-handed version later.
* All UK letters are 1 or 2 keys maximum.
* Should be able to replace a keyboard, a mouse, maybe a media remote.

## Editing
Layout editable in the amazing https://nickcoutsos.github.io/keymap-editor/ 

## History
I started with Ardux, as that (and it's predecessor Artsey) were the layouts that made me realise that you can accomplish a LOT with 8 keys. I implemented about 95% of Ardux on a Keybow 2040, and I learned a lot by doing it. There were some things, though, that I wanted to make better for me.

I noticed that a few of the two-key combinations available weren't being used. I did some rough calculations and realised I could represent every UK letter with one or two keys, so didn't need the 3 keys that are used for some in Ardux. \
I also realised that I type \<space\> more than any other character, so using a four-key combination for this wasn't ideal.

I did some quick analysis of which letters/characters I type most (this is a me thing) and the top 8 were (in some kind of order) \<space\> A E I N O R T \
So - those are the ones I wanted on my single-keys. I thought it would be good to have \<space\> on a pinkie, and tried a few different word combinations before settling on RAIN \<space\>TOE \
I had to move S and Y into other slots, and then for every other letter that was more than two keys, I found a two-key combination. I made sure to keep backspace and delete as two-key combinations too. I use backspace a lot, especially when learning new layouts. I don't use delete that often, but it felt weirdly wrong to move it.

I then defined (and redefined) lots of the symbols. Many of these do take 3 key-presses, but they avoid the need for a dedicated Symbols layer. \
I've aimed to be symmetric where possible: left and right brackets are broadly similar, slash and backslash are "opposites" of each other. \
Some, I'll admit, are just "leftovers", and if anyone has a better suggestion for these, I am happy to take it!

## Mods
Then mods - I quite liked the way I implemented them on the Keybow, even though I couldn't do the whole "light up the modifiers" on the Paintbrush. I've stuck with that method though - transient layer where you can either turn on the sticky version of a modifier (next keypress only) or by holding you can force the modifier to be stuck down. Mostly handy for selecting text, I guess.

## Arrows and Mouse
Arrows and Mouse: I found the Ardux way of getting to these clunky to be honest, so these are now transient layers accessed by holding bottom left and bottom right respectively.

## Numbers
Numbers: I've copied Ardux mostly, although instead of comma and full-stop/period being dedicated within Numbers, they are universal across both the standard and numeric key pad, as well as every other symbol.

## Bluetooth
Bluetooth: pretty much the same as Ardux. I'm using the excellent online ZMK Keymap Editor, which only goes up to 5 Bluetooth Slots, so that's the main difference.

## Layers
Layers: I set up a dedicated layer-switch layer on another keyboard and it works really well for me. In my head it's a bit like the bit of Nightmare Before Christmas where there are a set of doors in front of you - or similar for Narnia. Anyway - you can get to numbers, switch on mouse or arrow mode more permanently or get to a few other layers.

## Functions
Functions: same as Numbers, but goes up to F12. Could add more, but honestly other than bespoke keyboard shortcuts I've never used F13+

## Media / Mobile
Media/Mob: this is for when I connect my keyboard to my phone. Might iterate this further, but the idea is that it should allow most navigation/functionality to work. I haven't got an Apple device, so that's untested

## Custom
Custom: put what you want here. Currently, for convenience, I've got a few keys that I'm testing, plus a key to put the keyboard into bootloader mode and one to reset it. 

## Documenting and working out keyboard combinations
Oh - and one thing that took me a while is to find a good way of representing keyboard combinations. I eventually found that braille characters (3 of them) and different sized spaces gave me something that I could use in a spreadsheet. That way I could check for duplicates and "missing" combos. In the end, Google's AI found a good way of displaying them using multiple rows, but I still like the braille method for spreadsheets.


## TODOs
* TODO: Switch out display renderer for a prettier one
* TODO: Right-handed? NIAR EOT :)
* TODO: https://zmk.dev/docs/hardware-integration/soft-off-setup 

## Combo map

### Combo Pattern Matrix

# Note: 
These work in my locale (UK English). They may or may not work in yours, 
and I apologise if they do not. I do not know how to convert to multi-locale,
and it is not a priority right now.

#### Base Layer
| Pattern Map | Key / Action |
| :---: | :--- |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | `A` |
| <pre>○ ○ ○ ○<br>● ○ ○ ●</pre> | `B` |
| <pre>○ ○ ○ ○<br>○ ○ ● ●</pre> | `C` |
| <pre>○ ● ○ ●<br>○ ○ ○ ○</pre> | `D` |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | `E` |
| <pre>○ ○ ● ●<br>○ ○ ○ ○</pre> | `F` |
| <pre>○ ● ● ○<br>○ ○ ○ ○</pre> | `G` |
| <pre>○ ○ ○ ○<br>○ ● ○ ●</pre> | `H` |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | `I` |
| <pre>● ● ○ ○<br>○ ○ ○ ○</pre> | `J` |
| <pre>○ ○ ○ ○<br>● ○ ● ○</pre> | `K` |
| <pre>● ○ ○ ○<br>● ○ ○ ○</pre> | `L` |
| <pre>○ ○ ○ ○<br>● ● ○ ○</pre> | `M` |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | `N` |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | `O` |
| <pre>● ○ ○ ○<br>○ ○ ● ○</pre> | `P` |
| <pre>● ● ○ ●<br>○ ○ ○ ○</pre> | `Q` (Legacy) |
| <pre>○ ● ○ ○<br>○ ○ ○ ●</pre> | `QU`|
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | `R` |
| <pre>○ ● ○ ○<br>● ○ ○ ○</pre> | `S` |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | `T` |
| <pre>○ ○ ○ ○<br>○ ● ● ○</pre> | `U` |
| <pre>● ○ ● ○<br>○ ○ ○ ○</pre> | `V` |
| <pre>● ○ ○ ●<br>○ ○ ○ ○</pre> | `W` |
| <pre>○ ● ○ ○<br>○ ○ ● ○</pre> | `X` |
| <pre>○ ○ ● ○<br>○ ○ ● ○</pre> | `Y` |
| <pre>○ ○ ● ○<br>● ○ ○ ○</pre> | `Z` |
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | Space |
| <pre>○ ● ○ ○<br>○ ● ○ ○</pre> | `!` |

#### Numbers
| Pattern Map | Key / Action | 
| :---: | :--- |
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | `1` |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | `2` |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | `3` |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | `4` |
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | `5` |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | `6` |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | `7` |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | `8` |
| <pre>● ○ ○ ○<br>○ ○ ○ ●</pre> | `9` |
| <pre>● ○ ○ ○<br>○ ○ ● ○</pre> | `0` |

#### Global commands/keys
On most layers:-
* Holding top left activates Modifier mode
* Holding top right activates the Layer switch mode
* Holding bottom left activates Arrow mode
* Holding bottom right activates Mouse mode

All of these are only active as long as you hold that key, and revert back to the previous layer afterwards.

There's also the special Bluetooth mode, activated as per the bottom row in this table.

| Pattern Map | Key / Action |
| :---: | :--- |
| <pre>○ ○ ● ○<br>○ ○ ○ ●</pre> | Backspace |
| <pre>○ ○ ● ○<br>○ ● ○ ○</pre> | Delete |
| <pre>○ ○ ○ ●<br>○ ○ ○ ●</pre> | Enter |
| <pre>○ ○ ○ ●<br>● ● ● ○</pre> | Caps Lock (legacy) |
| <pre>● ● ○ ○<br>● ○ ○ ○</pre> | `Ctrl + X` (Cut) |
| <pre>● ○ ● ○<br>● ○ ○ ○</pre> | `Ctrl + C` (Copy) |
| <pre>● ○ ○ ●<br>● ○ ○ ○</pre> | `Ctrl + V` (Paste) |
| <pre>● ○ ○ ○<br>● ● ○ ○</pre> | `Ctrl + Z` (Undo) |
| <pre>● ○ ○ ○<br>● ○ ● ○</pre> | `Ctrl + Y` (Redo) |
| <pre>● ○ ○ ○<br>● ○ ○ ●</pre> | `Ctrl + W` (Close Window) |
| <pre>○ ● ● ●<br>○ ○ ○ ○</pre> | Tab |
| <pre>○ ● ○ ○<br>● ○ ○ ●</pre> | Print Screen |
| <pre>● ● ● ○<br>○ ○ ○ ○</pre> | Escape |
| <pre>○ ○ ● ○<br>● ○ ○ ●</pre> | Page Up |
| <pre>● ○ ○ ●<br>○ ○ ● ○</pre> | Page Down |
| <pre>○ ○ ● ●<br>○ ○ ● ●</pre> | Non-US Hash (`#`) |
| <pre>● ● ○ ○<br>● ● ○ ○</pre> | Asterisk (`*`) |
| <pre>○ ● ● ○<br>○ ○ ○ ●</pre> | Question Mark (`?`) |
| <pre>○ ○ ● ○<br>○ ● ○ ●</pre> | At Symbol (`@`) |
| <pre>● ○ ○ ●<br>● ○ ○ ●</pre> | Go to Bluetooth Layer |

#### Symbols that work across Base and Numbers layers
| Pattern Map | Key / Action | Active Layers |
| :---: | :--- | :--- |
| <pre>○ ○ ○ ●<br>○ ○ ● ○</pre> | Full Stop (`.`) | Base Layer, Numbers |
| <pre>○ ○ ○ ●<br>○ ● ○ ○</pre> | Comma (`,`) | Base Layer, Numbers |
| <pre>○ ● ○ ●<br>● ○ ○ ○</pre> | Plus Sign (`+`) | Base Layer, Numbers |
| <pre>● ○ ○ ○<br>○ ● ● ○</pre> | Percent (`%`) | Base Layer, Numbers |
| <pre>○ ● ● ○<br>● ○ ○ ○</pre> | Equals Sign (`=`) | Base Layer, Numbers |
| <pre>● ○ ○ ○<br>○ ● ○ ○</pre> | Hyphen (`-`) | Base Layer, Numbers |
| <pre>○ ○ ○ ●<br>○ ● ● ○</pre> | Single Quote (`'`) | Base Layer, Numbers |
| <pre>○ ○ ● ○<br>● ● ○ ○</pre> | Double Quote (`"`) | Base Layer, Numbers |
| <pre>○ ○ ○ ●<br>● ○ ○ ○</pre> | Slash (`/`) | Base Layer, Numbers |
| <pre>● ○ ○ ○<br>○ ○ ○ ●</pre> | Non-US Backslash (`\`) | Base Layer, Numbers |
| <pre>○ ○ ○ ○<br>● ● ● ○</pre> | Semicolon (`;`) | Base Layer, Numbers |
| <pre>○ ○ ○ ○<br>○ ● ● ●</pre> | Colon (`:`) | Base Layer, Numbers |
| <pre>○ ○ ● ●<br>● ○ ○ ○</pre> | Smart Normal Brackets (`()◀`) | Base Layer, Numbers |
| <pre>○ ○ ○ ○<br>● ○ ● ●</pre> | Right Normal Bracket (`)`) | Base Layer, Numbers |
| <pre>● ○ ● ●<br>○ ○ ○ ○</pre> | Smart Square Brackets (`[]◀`) | Base Layer, Numbers |
| <pre>● ○ ○ ○<br>○ ○ ● ●</pre> | Right Square Bracket (`]`) | Base Layer, Numbers |
| <pre>● ● ○ ○<br>○ ○ ○ ●</pre> | Smart Curly Brackets (`{}◀`) | Base Layer, Numbers |
| <pre>○ ○ ○ ○<br>● ● ○ ●</pre> | Right Curly Bracket (`}`) | Base Layer, Numbers |
| <pre>● ○ ○ ●<br>○ ● ○ ○</pre> | Tilde (`~`) | Base Layer, Numbers |
| <pre>● ○ ● ○<br>○ ○ ○ ●</pre> | Pipe (`\|`) | Base Layer, Numbers |
| <pre>○ ● ○ ●<br>○ ○ ● ○</pre> | Ampersand (`&`) | Base Layer, Numbers |
| <pre>○ ○ ● ●<br>○ ● ○ ○</pre> | Pound Symbol (`£`) | Base Layer, Numbers |
| <pre>○ ● ○ ○<br>○ ○ ● ●</pre> | Dollar Sign (`$`) | Base Layer, Numbers |
| <pre>○ ○ ○ ●<br>● ○ ● ○</pre> | Underscore (`_`) | Base Layer, Numbers |
| <pre>● ● ○ ○<br>○ ○ ● ○</pre> | Negation (`¬`) | Base Layer, Numbers |
| <pre>○ ● ○ ○<br>● ● ○ ○</pre> | "Broken Pipe" (`¦`) | Base Layer, Numbers |
| <pre>○ ○ ○ ●<br>● ● ○ ○</pre> | Backtick (`` ` ``) | Base Layer, Numbers |
| <pre>● ○ ● ○<br>○ ● ○ ○</pre> | Less Than (`<`) | Base Layer, Numbers |
| <pre>○ ● ○ ○<br>● ○ ● ○</pre> | Greater Than (`>`) | Base Layer, Numbers |

#### Function key layer
| Pattern Map | Key / Action |
| :---: | :--- |
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | `F1` |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | `F2` |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | `F3` |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | `F4` |
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | `F5` |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | `F6` |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | `F7` |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | `F8` |
| <pre>● ○ ○ ○<br>○ ○ ○ ●</pre> | `F9` |
| <pre>● ○ ○ ○<br>○ ○ ● ○</pre> | `F10` |
| <pre>● ○ ○ ○<br>○ ● ○ ○</pre> | `F11` |
| <pre>● ○ ○ ○<br>● ○ ○ ○</pre> | `F12` |

#### Media / mobile layer
| Pattern Map | Key / Action |
| :---: | :--- |
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | Back |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | Full screen |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | Home |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | Volume up | 
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | Rewind |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | Hold:Play, Tap: Play/Pause |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | Fast Forward |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | Volume Down | 
| <pre>● ○ ● ○<br>○ ○ ○ ○</pre> | Mouse Scroll Up |
| <pre>● ○ ○ ○<br>○ ○ ● ○</pre> | Mouse Scroll Down |
| <pre>● ○ ○ ●<br>○ ○ ○ ○</pre> | Media Forwards |
| <pre>○ ○ ○ ○<br>○ ● ● ○</pre> | Switch Display for Window |
| <pre>○ ○ ● ○<br>○ ● ○ ○</pre> | Virtual Desktop Left |
| <pre>○ ● ○ ○<br>○ ○ ● ○</pre> | Virtual Desktop Right |

#### Custom
| Pattern Map | Key / Action |
| :---: | :--- |
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | Win-tab |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | Turn off screen* |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | Not working: Soft Off |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | \<TBC\> |
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | \<TBC\> |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | Bootloader |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | Hold: Toggle Alt, Tap: Tab |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | Reboot keyboard |

*note: screen cannot be turned on again without power-cycling or doing a System Reset (E)

#### Arrows
| Pattern Map | Key / Action | 
| :---: | :--- |
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | \<TBC\> |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | Home key (text) |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | Up arrow |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | End key (text) |
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | N/A |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | Left arrow |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | Down arrow |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | Right arrow |
| <pre>○ ○ ● ○<br>○ ○ ● ○</pre> | Page Up |
| <pre>○ ○ ○ ○<br>○ ● ○ ●</pre> | Page Down |

#### Mouse
| Pattern Map | Key / Action | 
| :---: | :--- |
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | Left click |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | Mouse move up |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | Right click |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | \<TBC\> |
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | Mouse move left |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | Mouse move down |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | Mouse move right |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | N/A |
| <pre>○ ● ○ ○<br>● ○ ● ○</pre> | Mouse scroll up | 
| <pre>○ ○ ○ ○<br>● ● ● ○</pre> | Mouse scroll down |
| <pre>○ ● ○ ○<br>● ● ○ ○</pre> | Mouse scroll left |
| <pre>○ ● ○ ○<br>○ ● ● ○</pre> | Mouse scroll right |

#### Bluetooth layer
| Pattern Map | Key / Action | 
| :---: | :--- |
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | Select 1st Bluetooth connection |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | Select 2nd Bluetooth connection |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | Select 3rd Bluetooth connection |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | Switch to Bluetooth |
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | Select 4th Bluetooth connection |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | Select 5th Bluetooth connection |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | Back to base layer |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | Switch to USB |
| <pre>○ ● ● ○<br>○ ● ● ○</pre> | Clear current Bluetooth Profile |

#### Modifiers
Bottom row is Shift, Ctrl, Alt, Win. Holding toggles that key to be held, tapping makes it sticky for the next key press only. You can stack sticky modifiers (e.g. Shift + Ctrl).

To clear all modifier toggles, use A

| Pattern Map | Key / Action | 
| :---: | :--- |
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | N/A |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | Clear all modifier toggles |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | \<TBC\> |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | \<TBC\>  |
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | Hold: Toggle Shift on, Tap: Sticky Shift |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | Hold: Toggle Ctrl on, Tap: Sticky Ctrl |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | Hold: Toggle Alt on, Tap: Sticky Alt |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | Hold: Toggle Win on, Tap: Sticky Win |

#### Layer select
Lets you go straight to a layer. Numbers, Functions, Media, Custom are only available from here. You can also get to Arrows or Mouse as substantive layers in case you are navigating around a lot.
| Pattern Map | Key / Action | 
| :---: | :--- |
| <pre>● ○ ○ ○<br>○ ○ ○ ○</pre> | Base  |
| <pre>○ ● ○ ○<br>○ ○ ○ ○</pre> | Numbers |
| <pre>○ ○ ● ○<br>○ ○ ○ ○</pre> | Functions |
| <pre>○ ○ ○ ●<br>○ ○ ○ ○</pre> | N/A |
| <pre>○ ○ ○ ○<br>● ○ ○ ○</pre> | Arrows |
| <pre>○ ○ ○ ○<br>○ ● ○ ○</pre> | Media/Mobile |
| <pre>○ ○ ○ ○<br>○ ○ ● ○</pre> | Custom |
| <pre>○ ○ ○ ○<br>○ ○ ○ ●</pre> | Mouse |


N/A means a key has not been overridden because it would interfere with the activation of the layer it is on. You could use the ones on the Arrows and Mouse layers if you are going via Layer Select if you like.

\<TBC\> means I just haven't assigned anything ... yet!