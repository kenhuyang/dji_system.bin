Known Md5s of files pulled from DJI updates, user contributed files, and exploits. 
https://github.com/MAVProxyUser/dji_system.bin/blob/master/MD5s.md 

To combine your own files do the following (using gnu-tar from brew if on OSX):
```
$ cp UniversalFireworksTar_dji_system.bin mavic_combined_700_root.bin 
gtar --concatenate --file mavic_combined_700_root.bin V01.03.0700_Mavic_dji_system.bin
$ tar tvf mavic_combined_700_root.bin

-rw-r--r--  0 root   staff      37 Jul  9 01:51 Burning0day.txt
lrwxr-xr-x  0 root   staff       0 Jul  9 01:51 symlink -> /data/.bin
-rwxr-xr-x  0 root   staff     517 Jul  9 01:51 symlink/grep
-rwxrwxrwx  0 0      users   55072 Jul 12 15:41 wm220_0305_v34.04.00.23_20161122.pro.fw.sig
-rwxrwxrwx  0 0      users 1537056 Jul 12 15:41 wm220_0306_v03.02.30.13_20170405.pro.fw.sig
-rwxrwxrwx  0 0      users   20768 Jul 12 15:41 wm220_1200_v01.09.00.00_20161204.pro.fw.sig
-rwxrwxrwx  0 0      users   20768 Jul 12 15:41 wm220_1201_v01.09.00.00_20161204.pro.fw.sig
-rwxrwxrwx  0 0      users   20768 Jul 12 15:41 wm220_1202_v01.09.00.00_20161204.pro.fw.sig
-rwxrwxrwx  0 0      users   20768 Jul 12 15:41 wm220_1203_v01.09.00.00_20161204.pro.fw.sig
-rwxrwxrwx  0 0      users   28416 Jul 12 15:41 wm220_1100_v01.00.07.24_20161206.pro.fw.sig
-rwxrwxrwx  0 0      users   43488 Jul 12 15:41 wm220_0803_v00.00.04.08_20170314.pro.fw.sig
-rwxrwxrwx  0 0      users 15180832 Jul 12 15:41 wm220_0100_v02.02.56.29_20170317.pro.fw.sig
-rwxrwxrwx  0 0      users 37489024 Jul 12 15:41 wm220_0100_v02.06.04.84_20170324_ca02.pro.fw.sig
-rwxrwxrwx  0 0      users    60128 Jul 12 15:41 wm220_0101_v02.06.04.84_20170324_ca02.pro.fw.sig
-rwxrwxrwx  0 0      users   196544 Jul 12 15:41 wm220_0101_v02.02.56.29_20170317.pro.fw.sig
-rwxrwxrwx  0 0      users    91584 Jul 12 15:41 wm220_0400_v01.50.12.01_20170414.pro.fw.sig
-rwxrwxrwx  0 0      users    26432 Jul 12 15:41 wm220_0804_v01.00.00.08_20170113.pro.fw.sig
-rwxrwxrwx  0 0      users  4142592 Jul 12 15:41 wm220_0907_v47.26.02.11_20170419.pro.fw.sig
-rwxrwxrwx  0 0      users 41515328 Jul 12 15:41 wm220_0801_v01.05.00.20_20170331.pro.fw.sig
-rwxrwxrwx  0 0      users  5320416 Jul 12 15:41 wm220_0802_v01.00.03.08_20170116.pro.fw.sig
-rwxrwxrwx  0 0      users  3052000 Jul 12 15:41 wm220_0805_v01.01.00.87_20170427.pro.fw.sig
-rwxrwxrwx  0 0      users    92096 Jul 12 15:41 wm220_0905_v00.00.01.04_20170301.pro.fw.sig
-rwxrwxrwx  0 0      users     5888 Jul 12 15:41 wm220.cfg.sig
```
You can see this file has BOTH the root, and the downgrade packaged together. 

You can also create your own single sig updates from the firm_cache
https://github.com/MAVProxyUser/firm_cache

```
iMac:firm_cache hostile$ mkdir test
iMac:firm_cache hostile$ cd test
iMac:test hostile$ cp ../wm220_0305_v34.04.00.23_20161122.pro.fw.sig ../V01.03.0900_Mavic_dji_system/wm220.cfg.sig .
iMac:test hostile$ tar cvf dji_system.bin *.sig
a wm220.cfg.sig
a wm220_0305_v34.04.00.23_20161122.pro.fw.sig
```

Example file:
MD5 (single_sig_test.tar) = 72e2bb6753aeb048946875a31e5a20a8

Push the above file with pyduml of course... 

This is the most up to date source of info on "rooting" DJI aircraft. Start here with questions
http://dji.retroroms.info 
