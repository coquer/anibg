## About: ##

With "anibg" you can put a XScreenSaver or a movie on your x11 desktop, you can see it as a "Windows DreamScene" pendant.

More precisely it is a frontend for the CLI application "Shantz-XWinWrap".
It works on Linux and could work on BSD and other unix based systems too, but I'm not sure, because I couldn't test it.

It supports the languages english and german.

<a href='http://www.youtube.com/watch?feature=player_embedded&v=t4ggNlqhDIc' target='_blank'><img src='http://img.youtube.com/vi/t4ggNlqhDIc/0.jpg' width='425' height=344 /></a>

## Installation: ##

### Ubuntu 10.04 and 10.10 ###

Just type this in your terminal:
```
wget http://anibg.googlecode.com/files/anibg_v0.2.0.deb && wget http://anibg.googlecode.com/files/shantz-xwinwrap_v0.3.deb && sudo dpkg -i anibg_v0.2.0.deb shantz-xwinwrap_v0.3.deb
```

### Compilation ###

You need "mono", "glade-sharp-2.0", "gtk-sharp-2.0", "glib-sharp-2.0"
and "notify-sharp" to run "anibg" and "make" to compile it.
"anibg" uses "Shantz-XWinWrap" which will be delivered with this package.
To use "Shantz-XWinWrap" you need "x11", "xext"
and "xrender" and their development files to compile it.
For movie support you need "MPlayer" and "FFmpeg".
Install some "XScreenSavers", else you won't have any
Screensaver to select.

Then type these commands in your terminal:
```
cd ~/
wget http://anibg.googlecode.com/files/anibg_v0.2.0.tar.gz
tar -xzvf anibg_v0.2.0.tar.gz
cd anibg_v0.2.0/src/
./configure
make
make install # Must be executed as root
```