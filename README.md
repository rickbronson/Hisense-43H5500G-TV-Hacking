  Hisense 43H5500G TV Hacking
==========================================

This is sort of a call for help on hacking a Hisense 43H5500G TV.  Someone in my neighborhood threw this TV out on the street with a badly cracked screen (it did not come with a remote).  I stuffed it into my bike trailer and brought it home to see what TV's these days have in them.  Surprisingly little it turns out.  I got excited when I found that it runs Linux but dismayed that I could not break into it.  The boot loader (some combination of Mboot and U-Boot) is locked down pretty tight.  What I'd really like to do is play around with the digital tuner.

  Chips used on this TV:

 - Main CPU:  Mstar MSD6683BQHT
 - WiFi: MT7668
 - eMMC: HS400

This seems to be an "Android TV".  See https://sites.google.com/view/droid-tv/ and https://wikidevi.wi-cat.ru/Android_TV https://exploitee.rs/index.php/Hisense_Android_TV

Here are some pictures I took:

Various "model" labels which makes it hard to find exactly what model this thing is.
![Hisense model](https://github.com/rickbronson/Hisense-43H5500G-TV-Hacking/blob/master/docs/hardware/hisense-model.png "Hisense model")

The bottom of the Mainboard
![MB-bottom](https://github.com/rickbronson/Hisense-43H5500G-TV-Hacking/blob/master/docs/hardware/MB-bottom2.png "MB-bottom")

The top of the Mainboard
![MB-top2](https://github.com/rickbronson/Hisense-43H5500G-TV-Hacking/blob/master/docs/hardware/MB-top2.png "MB-top")

The top of the Mainboard with the giant heatsink that covers the CPU removed.
![MB-hisense.jpg](https://github.com/rickbronson/Hisense-43H5500G-TV-Hacking/blob/master/docs/hardware/MB-hisense.jpg "MB-hisense.jpg")

The CPU with heatsink removed.
![MB chips](https://github.com/rickbronson/Hisense-43H5500G-TV-Hacking/blob/master/docs/hardware/MB-chips.jpg "MB chips")

  Also in the docs/hardware folder there are some pdf's that seem to have some info on the design of TV's like this one.

```
Manual_de_tecnico_91PLD32HS7A.pdf
Manual_de_tecnico_91PLD32HS9A.pdf
Manual_tecnico_91PLD32HS9B.pdf
```

 I hooked up a TTL serial port to the RX TX pins (see photos's above) and got a boot log (see boot3.log) but there was no was of interrupting the boot process and gaining control.

Comments/suggestions

  Please contact me at rick AT efn DOT org
