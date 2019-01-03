# Tiny HTTP Proxy in Python

I wrote a tiny HTTP proxy in Python in September, 2001.  It was for
Python 2.1 on BeOS R5 originally, and has been working well ever since
in every version of Python 2 on almost every platform, including macOS
and Windows 2000/XP/7/10.  I posted it to _python-list_ on 17 June,
2003.  It was once available at
<http://www.oki-osk.jp/esc/python/proxy/> from 2006 to 2017.

Now I have revised the proxy so that it can run on both Python 2.7 
and Python 3.7.

I hope the code of the proxy is short enough to be self-explanatory.
If your LAN is narrow or unstable, it would be better to increase the
default value of `max_idling` in `_read_write()` from 20 to, say, 100.

```
$ python ./TinyHTTPProxy.py
Any clients will be served...
Serving HTTP/1.0 on 0.0.0.0 port 8000 ...

```
