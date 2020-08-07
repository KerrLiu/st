# Simple Terminal (kerr build)

Make according to Luke Smith configuration


## keybind

|     hotkey    |     info      |
|-------:-------|-------:-------|
|    MODKEY+c   |   clipcopy    |
|    MODKEY+v   |   clippaste   |
|    MODKEY+p   |   selpaste    |
|    MODKEY+k   |   kscrollup   |
|    MODKEY+j   |   kscrolldown |
|    MODKEY+u   |   kscrollup   |
|    MODKEY+d   |   kscrolldown |
|    MODKEY+l   |   openurlcmd  |
|    MODKEY+y   |   copyurlcmd  |
|    MODKEY+o   |   copyoutput  |
|   TERMMOD+K   |   zoom.f+1    |
|   TERMMOD+J   |   zoom.f-1    |


## Patches

+ alpha
+ anysize
+ clipboard
+ font2
+ iso14755
+ ligatures
+ scrollback
+ vertcenter
+ w3m
+ xresources



## suckless.org info

st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

