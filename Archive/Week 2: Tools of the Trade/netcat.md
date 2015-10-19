# netcat

netcat is a tool for creating, reading from and writing to network connections.

## Examples

### Turning a process into a server

```
$ nc -l -p 1234 -e /bin/sh
```
```
$ nc 192.168.1.2 1234
ls -las
total 4288
4 drwxr-xr-x 15 imsovain users 4096 2009-02-17 07:47 .
4 drwxr-xr-x  4 imsovain users 4096 2009-01-18 21:22 ..
8 -rw-------  1 imsovain users 8192 2009-02-16 19:30 .bash_history
4 -rw-r--r--  1 imsovain users  220 2009-01-18 21:04 .bash_logout
...
```

(more: http://en.wikipedia.org/wiki/Netcat)

### Sending a file from A to B

B:
```
nc -l -p 1234 > out.file
```

A:
```
nc -w 3 [destination] 1234 < out.file
```

(more: http://nakkaya.com/2009/04/15/using-netcat-for-file-transfers/)
