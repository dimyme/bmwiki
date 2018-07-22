* Reduce the "log level" to have smaller "debug.log" files, or none at all.
edit a text file "logger.dat" [accordingly](https://docs.python.org/2/library/logging.config.html#logging.config.fileConfig): how to [do it](https://bitmessage.org/forum/index.php?topic=4820.msg11163#msg11163)  to reduce logging,  edit a text file .../src/logger.dat   with content:


[logger_root]

level=NOTSET

handlers=handler_null

[formatters]

keys =

[formatter_null]

wtf=null

[handlers]

keys =

[handler_null]

class =

[loggers]

keys = root




***




***
### switch to HTML view automatically

in regular pyBM you must switch over manually, because of security concerns. http://bitmessage.mybb.im forum has more info on how to do that automatically, just 3 lines must be adapted. 

Those places in the python code should be marked ###USER_FEATURE there are a couple of them in existence, such as modified number of connections etc.. find more info in the 3 forums out there (UBF and the others).