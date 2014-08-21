mkrelease
=========

Creates a Capistrano like directory structure

Usage
=====

```bash
$ mkrelease -k 3 build
$ ls -ln build
total 4
drwxr-xr-x 2 1000 100 4096 Aug 21 12:28 20140821122840
lrwxrwxrwx 1 1000 100   14 Aug 21 12:28 current -> 20140821122840

$ for i in $(seq 10); do ./mkrelease -k3 build; done
$ ls -l build 
total 12
drwxr-xr-x 2 gchain users 4096 Aug 21 12:28 20140821122840
drwxr-xr-x 2 gchain users 4096 Aug 21 12:30 20140821123055
drwxr-xr-x 2 gchain users 4096 Aug 21 12:30 20140821123056
lrwxrwxrwx 1 gchain users   14 Aug 21 12:30 current -> 20140821123056
```
