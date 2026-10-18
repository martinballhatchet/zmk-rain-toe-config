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
Media+Mob: this is for when I connect my keyboard to my phone. Might iterate this further, but the idea is that it should allow most navigation/functionality to work. I haven't got an Apple device, so that's untested

## Custom
Custom: put what you want here. Currently, for convenience, I've got a few keys that I'm testing, plus a key to put the keyboard into bootloader mode and one to reset it. 

## Documenting keyboard combinations
Oh - and one thing that took me a while is to find a good way of representing keyboard combinations. I eventually found that braille characters (3 of them) and different sized spaces gave me something that I could use in a spreadsheet. That way I could check for duplicates and "missing" combos.


## TODOs
* TODO: Switch out display renderer for a prettier one
* TODO: Can we clear toggles?
* TODO: Right-handed? NIAR EOT :)
* TODO: https://zmk.dev/docs/hardware-integration/soft-off-setup 

## Rough map of combos

Below is a rough combo map - hopefully will produce a better one later.

```
rain toe
⎸ ⠁  ⎸A
⎸⡀  ⡀⎸	B
⎸  ⡀⡀⎸	C
⎸ ⠁ ⠁⎸	D
⎸   ⡀⎸E
⎸  ⠁⠁⎸	F
⎸ ⠁⠁ ⎸	G
⎸ ⡀ ⡀⎸	H
⎸  ⠁ ⎸I
⎸⠁⠁  ⎸	J
⎸⡀ ⡀ ⎸	K
⎸⡁   ⎸L
⎸⡀⡀  ⎸	M
⎸   ⠁⎸N
⎸  ⡀ ⎸O
⎸⠁ ⡀ ⎸	P
⎸⠁⠁ ⠁⎸	Q
⎸⠁   ⎸R
⎸⠁⡀  ⎸	S
⎸ ⡀  ⎸T
⎸ ⡀⡀ ⎸	U
⎸⠁ ⠁ ⎸	V
⎸⠁   ⠁ ⎸	W
⎸ ⠁⡀ ⎸	X
⎸  ⡁ ⎸Y
⎸⡀ ⠁ ⎸	Z
⎸⡁ ⠁ ⎸	Ctrl C
⎸⡁  ⠁⎸	Ctrl V
⎸⡁  ⡀⎸	Ctrl W
⎸⡁⠁  ⎸	Ctrl X
⎸⡁⡀  ⎸	Ctrl Y
⎸⡁ ⡀ ⎸	Ctrl Z
⎸  ⠁⡀⎸	Backspace
⎸⡀⡀⡀⠁⎸	Caps Lock
⎸   ⡁⎸Enter
⎸⠁⠁⠁ ⎸	Escape
⎸ ⡀⠁ ⎸	Forward delete
⎸⠁ ⡀⠁⎸	Page Down
⎸⡀ ⠁⡀⎸	Page Up
⎸⡀⠁ ⡀⎸	Print Screen
⎸⡀   ⎸Space
⎸ ⠁⠁⠁⎸	Tab
⎸⡁  ⡁⎸	BT Layer
⎸ ⡁⡁ ⎸	Clear BT Profile
⎸ ⠁ ⡀⎸	QU
⎸⡀ ⡀⠁⎸	_
⎸⡀⠁  ⎸	-
⎸ ⡀ ⠁⎸	,
⎸⡀⡀⡀ ⎸	;
⎸ ⡀⡀⡀⎸	:
⎸ ⡁  ⎸!
⎸ ⠁⠁⡀⎸	?
⎸  ⡀⠁⎸	.
⎸ ⡀⡀⠁⎸	'
⎸⡀⡀⠁ ⎸	"
⎸⡀ ⠁⠁⎸	(
⎸⡀ ⡀⡀⎸	)
⎸⠁ ⠁⠁⎸	[
⎸⠁ ⡀⡀⎸	]
⎸⠁⠁ ⡀⎸	{
⎸⡀⡀ ⡀⎸	}
⎸ ⡀⠁⡀⎸	@
⎸⡁⡁  ⎸	*
⎸⡀  ⠁⎸	/
⎸⠁  ⡀⎸	\
⎸ ⠁⡀⠁⎸	&
⎸  ⡁⡁⎸	#
⎸⠁⡀⡀ ⎸	%
⎸⡀⡀ ⠁⎸	`
⎸⡀⠁ ⠁⎸	+
⎸⠁⡀⠁ ⎸	<
⎸⡀⠁⠁ ⎸	=
⎸⡀⠁⡀ ⎸	>
⎸⠁⠁⡀ ⎸	¬
⎸⠁ ⠁⡀⎸	|
⎸⡀⡁  ⎸	¦
⎸⠁⡀ ⠁⎸	~
⎸ ⠁⡀⡀⎸	$
⎸ ⡀⠁⠁⎸	£
	
```
