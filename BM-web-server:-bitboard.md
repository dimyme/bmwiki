an image board on top of Bitmessage and thought I'd share it with the community. Although it's still somewhat basic, it does have a fair bit of features already, although they do come with some drawbacks. Basically, once you're running Bitmessage with the API enabled, you can then run bitboard, which will connect to the API, and load all your channels into a friendly 4chan-style image board. Since this is running in your browser, it is worth noting that it does increase the attack surface. I'd suggest disabling javascript if you are worried about that- bitboard uses only minimal uses of JS and is still fully usable without it. It also uses the python 'bleach' module in an attempt to prevent html/js from being injected. I spent a fair bit of work implementing popups and such using CSS to avoid reliance on JS based features. A few features - Automatically groups message into threads based on the post subject. - Automatically (best-effort) parses base64 images and inserts them into threads. - Simple UI for joining new chans. - 3 different themes. - Deleting posts and entire threads. Messages you send through bitboard are encoded into a JSON blob, so is a bit unfriendly for non-users, although posts are still somewhat readable. However, Bitboard will automatically distinguish between posts sent through bitboard vs the official client, and display both properly. Not sure if I will maintain it much, it's more of a proof of concept type thing. Just thought you all might be interested. 

 https://github.com/michrob/bitboard