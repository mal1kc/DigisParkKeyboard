DigisparkKeyboard library with multiple layout support
======================================================
 
Based on DigisparkKeyboard library

This library allows an Digispark board with Attiny85 act as a Keyboard.

For more information about this boards visit http://digistump.com/category/1

Modified by Ernesto Sanchez to support multiple keyboard layouts

Modified by Mümin Köykıran to support Turkish keyboard layouts 

Modified by malik kökçan to support media keys with consumer page descriptors

Supported layouts:
* tr_tr
* be_be
* cz_cz
* da_dk
* de_de
* en_us (default)
* es_es
* fi_fi
* fr_fr
* it_it
* pt_pt

__NOTE1:__ Only en_us and es_es are tested at july 2017.
__NOTE2:__ tr_tr tested at March 2018. The result is perfect.

Download and installation
=========================
- Click "Clone or download" -> "Download ZIP"
- Unzip downloaded file in Arduino/libraries/ directory
- Maybe you need to use this directory (C:\Users\Mümin Köykıran\AppData\Local\Arduino15\packages\digistump\hardware\avr\1.6.7\libraries\) in your PC

Use
===
To configure the keyboard layout it just add #define kbd_lang after #include "DigiKeyboard.h"

Example:
```
#define kbd_tr_tr
#include "DigiKeyboard.h"
```

You can use:
* kbd_tr_tr
* kbd_be_be
* kbd_cz_cz
* kbd_da_dk
* kbd_de_de
* kbd_en_us
* kbd_es_es
* kbd_fi_fi
* kbd_fr_fr
* kbd_it_it
* kbd_pt_pt

If none is especified en_us is used by default.

Version History
===============
```
(Date format: DD/MM/YYYY)
* 8/7/2017 First commit
* 27/2/2023 forked from ernesto-xload repo + added media keys (consumer page)
```

TO DO
=====
- Implement a solution for extended ascii characters for all layouts
- fix media keys bugs

Contact
=======
Open an issue, ask me on gihub [@mal1kc](http://www.github.com/mal1kc/)

Resources used by mal1kc
=======

[custom usb hid device descriptor](https://notes.iopush.net/blog/2016/custom-usb-hid-device-descriptor-media-keyboard/)

[usb hid codes](https://www.usb.org/hid)

[Change USB VID & PID on Digispark](https://blog.spacehuhn.com/digispark-vid-pid)
