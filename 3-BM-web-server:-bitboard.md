an image board - i.e. **a website on top of Bitmessage** https://github.com/michrob/bitboard 
***
quick install of Bitmessage and bitboard in a bash Konsole: [bash  installer Script](https://pastebin.com/print/HrLtCKaj)

_**pastebin.com/HrLtCKaj**_

***
If someone puts a BitBoard on public internet, please post the link here: _____________ , thanks.

Although it's still somewhat basic, it does have a fair bit of features already, although they do come with some drawbacks. Basically, once you're running Bitmessage with the API enabled, you can then run bitboard, which will connect to the API, and load all your channels into a friendly 4chan-style image board. 


Since this is running in your browser (e.g. **firefox**), it is worth noting that it does increase the attack surface. Possible to set up www-facing like www.BEAMSTAT.com


I'd suggest disabling javascript if you are worried about that - bitboard uses only minimal uses of JS and is still **fully usable without JS** (like all 4chan-like picture-boards). 

It also uses the python 'bleach' module in an attempt to prevent html/js from being injected. I spent a fair bit of work implementing popups and such using CSS to avoid reliance on JS based features. A few features 

*  Automatically groups message into threads based on the post subject. 
*  Automatically (best-effort) parses base64 images and inserts them into threads. 
*  Simple UI for joining new chans. 
*  3 different themes. 
*  Deleting posts and entire threads. 


Messages you send through bitboard are encoded into a _JSON_ blob, so is a bit unfriendly for users of the regular pyBM, although posts are still somewhat readable in normal pyBM and BEAMSTAT.com . However, Bitboard will automatically distinguish between posts sent through bitboard vs. the official client "pyBM", and display both properly. 

Not sure if I will maintain it much, it's more of a proof of concept type thing - but already bitboard is better than BMF, which has refreshing trouble a lot. _Essentially, BMF is a lot less interesting since the BitBoard era was ushered in._

**please fork & contribute!**        https://github.com/michrob/bitboard 

***
You can expose bitboard to the darkweb on an .onion-www-site using this single bash [script]( http://fossilrepos.sourceforge.net/srv.fsl/450/wiki?name=Leeres+Fossil+Repo), then you run a website like http://beamstat.com

TODO: use the debian server deployment script for pyBM which s.o. posted somewhere and add BB to it for super-fast auto-deploy of a BM website on a headless remote server.