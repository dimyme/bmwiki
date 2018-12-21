### noteworthy projects to be used in conjunction with BitMessage:
***
easy **menu to install pyBm and bitboard** (a bash script to run in xterm) in just 10 seconds for GNU-Linux is [here](https://gist.githubusercontent.com/KM-200/715f8847bd24b9e6ebb90e0a64d5149a/raw/747df7a695b09aa5e133d6a7d86c6387ab10348e/bm_menu.sh) and [here](http://fossilrepos.sourceforge.net/srv.fsl/450/wcontent?all=1) . The latter link points to a censorship-free wiki. Unfortunately, some Bitmessage sites suffer from censorship beyond the control of BM admins and developers. [python2-sip-pyqt4](https://gitlab.com/inemum/inemum_archlinux/raw/master/python2-sip-pyqt4/PKGBUILD) may be required too (undetected by checkdeps.py currently).

You can expose bitboard to the darkweb on an .onion-www-site using this single [bash script](http://fossilrepos.sourceforge.net/srv.fsl/450/wiki?name=Leeres+Fossil+Repo), then you run a website like http://beamstat.com
***
easily modify pyBM in text mode (i.e. --curses mode): https://github.com/dimyme/PyBitmessage/blob/v0.6/src/bitmessagecurses/modding/__init__.py


***
https://github.com/michrob/bitboard web interface, use BM via firefox, better than _BitMessageForum_

https://github.com/majestrate/BitMessageForum web interface, bitboard is better though


***
use ThunderBird to read BM:  https://github.com/Arceliar/bmwrapper   

runs a localhost:12344 pop3-mailserver for BM so ThunderBird is being used to read & write BM besides the original GUI. The "**claws**" mail-app can be used too, which has nice a python plug-in to have claws scripted and modified.

puts everything in one huge INBOX initially. Use filters in ThuBi to separate the [chan]nels. 

Gives you some more features, e.g. sort BM by size, which you cannot do in pyBM. No full threaded view, though.
***
https://github.com/yamamushi/bmfec

https://github.com/TheKysek/MiNode

https://github.com/bitchan/bitmessage

https://github.com/Thomas-Astade/bitmessaged

https://github.com/Dissem/Abit
Bitmessage Client for Android

bash script to deploy BM on a debian server as [daemon](https://github.com/r51n/auto-bitmessage) 

spam filter and BM [API](https://github.com/torifier/PyBitmessage/tree/master/bitmessage-API/spamfilter)

"[mammoth](https://gist.github.com/anonymous/925445ea97d7bc8622d0b706469adc42)" , a keys.dat file with 1000+ chans

a [chan generator](http://bitmessage.mybb.im/viewtopic.php?id=30%23p106) in python, [archived here](http://web.archive.org/web/20180723031649/http://bitmessage.mybb.im/viewtopic.php?id=30%23p222) .

bash menu to use a one-time-pad additional encryption with BM: pyBM-sigoa
