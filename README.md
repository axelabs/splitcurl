Curl can accelerate a download of a file by splitting it into parts:
```
$ man curl |grep -A2 '\--range'
      -r/--range <range>
         (HTTP/FTP/SFTP/FILE) Retrieve a byte range (i.e a partial docu-
         ment) from a HTTP/1.1, FTP or SFTP server or a local FILE.
```
Splitcurl is a bash wrapper that allows you to specify how many parts to split the download into:
```
$ ./splitcurl
http://mirrors.rutgers.edu/archlinux/iso/2012.10.06/archlinux-2012.10.06-dual.iso
100 Downloading archlinux-2012.10.06-dual.iso in 100 parts: 435159040 / 435159040 bytes @ 22366 kb/s (100%).
Files done! 
```
Usage:
```
       splitcurl URL [SPLITNUM(4)]
```
\> [Download it!](https://raw.githubusercontent.com/axelabs/splitcurl/master/splitcurl) <
