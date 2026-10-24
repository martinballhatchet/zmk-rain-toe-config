Things that I have tried and backed out:

* EP_TOG / EP_ON don't work to turn on external power. You can turn it off, but have to reset to turn it back on
* Can't see a way to disable Bluetooth
* Considered adding ZMK Studio support, but a LOT of this keyboard layout is managed via combos, so there is very limited value in this.
ine
* I really don't like the way ZMK keeps all paired BT devices connected. Looked at a few ways of fixing it, but none work. Tried changing each of the BT_MAX settings - neither of those work the way I need them too. Tried disconnecting all but the current bluetooth connection - nope, they definitely disconnect ... but then reconnect immediately. For each of those, I tried flashing a settings_reset firmware inbetween - still no difference. It looks like it's a known issue in the ZMK layer (not the Zephyr layer) that is unlikely to get fixed
