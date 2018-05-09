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






