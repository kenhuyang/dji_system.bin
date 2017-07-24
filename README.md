# dji_system.bin
DJI is currently in violation of GPL... these binaries are intended to be distributed to end users that have purchased either an nspire2, Goggles, Mavic, Spark, or P4 variant drone,and are seeking to downgrade their aircraft back to its factory state. 

Update:
On Jul 18, 2017, at 10:30 AM, Bruce Perens wrote:
"Thank you (and whoever else helped) very much for the detailed examination which I see on your GIT repository. 
Please inform the DJI community that this morning I have written to DJI legal regarding the problem. I will inform you if they respond"

![Initial contact and refusal to supply](https://pbs.twimg.com/media/DEt61OTUAAAOd7j.jpg)

![Second Attempt with internal help!](https://pbs.twimg.com/media/DEt61X1VYAA37KC.jpg)

![A month later... still nothing](https://pbs.twimg.com/media/DEt61RpU0AA2QZ9.jpg)

![then we learn P0V tried too...](https://pbs.twimg.com/media/DE168EuVoAA9RTc.jpg)

The initial GPL violation was noticed in an AES implementation added to BusyBox ftpd (running inside the drone components)
https://github.com/MAVProxyUser/DJI_ftpd_aes_unscramble

This issue was subsequently highlighted when the "tar -C" directory traveral issue was revealed in the busybox tar used by DJI update processes
https://github.com/MAVProxyUser/P0VsRedHerring/
https://github.com/MAVProxyUser/P0VsRedHerring/blob/master/RedHerring.rb#L30
https://bugs.busybox.net/attachment.cgi?id=6211&action=diff
https://bugs.busybox.net/show_bug.cgi?id=8411

Now about the GPL binaries and accompanying source... 

![GPL Violation](https://pbs.twimg.com/media/DE1Bq1zU0AEG2lx.jpg)

https://www.gnu.org/licenses/gpl-faq.en.html
```
“GPL gives a person permission to make & redistribute copies of the program if & when that person chooses to do so”
https://www.gnu.org/licenses/gpl-faq.en.html#CanIDemandACopy
“You can charge people a fee to get a copy from you. You can't require people to pay you when they get a copy from someone else.”
“if someone pays your fee and gets a copy, the GPL gives them the freedom to release it to the public, with or without a fee”
“The GPL says that anyone who receives a copy from you has the right to redistribute copies, modified or not.”
https://www.gnu.org/licenses/gpl-faq.en.html#DoesTheGPLAllowNDA
“If it depends on a nonfree library to run at all, it cannot be part of a free operating system such as GNU;”
https://www.gnu.org/licenses/gpl-faq.en.html#FSWithNFLibs
“If they form a single combined program then the main program must be released under the GPL”
You cannot incorporate GPL-covered software in a proprietary system.”
https://www.gnu.org/licenses/gpl-faq.en.html#GPLInProprietarySystem
“you must make sure that the free and nonfree programs communicate at arms length”
https://www.gnu.org/licenses/gpl-faq.en.html#GPLInProprietarySystem
“Can I release a modified version of a GPL-covered program in binary form only?”
https://www.gnu.org/licenses/gpl-faq.en.html#ModifiedJustBinary
“The exception for the case where you received a written offer for source code is quite limited.”
“must be open to everyone who has a copy”
“This is a well-meaning request, but this method of providing the source doesn't really do the job.”
https://www.gnu.org/licenses/gpl-faq.en.html#DistributingSourceIsInconvenient
“As long as you make the source and binaries available so that the users can see what's available and take what they want”
“Complete corresponding source means the source that the binaries were made from”
https://www.gnu.org/licenses/gpl-faq.en.html#MustSourceBuildToMatchExactHashOfBinary
“If the version has been released elsewhere, then the thief probably does have the right to make copies and redistribute them under the GPL”
https://www.gnu.org/licenses/gpl-faq.en.html#TradeSecretRelease
“If a company distributes a copy to you and claims it is a trade secret, the company has violated the GPL” 
https://www.gnu.org/licenses/gpl-faq.en.html#TradeSecretRelease
```

Words from the ever so wise Tridge of ArduPilot "Malicious? Fight them"
https://www.samba.org/~tridge/gplv3_sydney.pdf
![GPL Violation](https://pbs.twimg.com/media/DE5eiumUIAAHpan.jpg)

As a simple example we can take Busybox:
![GPL Violation](https://pbs.twimg.com/media/DE5caDoU0AArLcC.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE5cKTgUAAAV-0J.jpg)

If this were the good ole days... they would be on the public shame wall.
https://web-beta.archive.org/web/20130116093247/http://busybox.net/shame.html
![GPL Violation](https://pbs.twimg.com/media/DE5eIdBXkAAjRy2.jpg)

Please contact FSF and ask for the GPL source code that DJI uses to be published. 
[![Fuck yeah](https://media.giphy.com/media/wi8Ez1mwRcKGI/giphy.gif)](https://www.youtube.com/watch?v=T437DdmFNPU)

http://www.fsf.org/licensing/compliance

Known Md5s of files pulled from DJI updates, user contributed files, and exploits. 
```
MD5 (UniversalFireworksTar_dji_system.bin) = 0e0b9d397ad132dc5af8ee37d1b2a5fd
MD5 (V01.00.0300_Spark_dji_system.bin) = bf81af1c10318e8549bb78b0fef85013
MD5 (V01.00.0330_I2_dji_system.bin) = 0a5c437812b91355c9ae0d4d28d505d1
MD5 (V01.00.0400_Spark_dji_system.bin) = 65f15f4cbe7d761459c7a09ebc660801
MD5 (V01.01.0010_I2_dji_system.bin) = 7d04f199bd872c9372fdebddbef3c404
MD5 (V01.01.0203_P4P_dji_system.bin) = 950ca897ee21cbb545f5e30ab198eaa7
MD5 (V01.02.0503_P4_dji_system.bin) = 96a52ebc0f9152fd9fd02566f60ade77
MD5 (V01.02.0602_P4_dji_system.bin) = 36e11566ae6e303ec5c407f9c0f6c382
MD5 (V01.03.0200_Mavic_dji_system.bin) = 3d27db82d7f7a5f6a5025ffa08aa89e8
MD5 (V01.03.0200_RC_Mavic_dji_system.bin) = 80e350c2c767fcf2a86c997edf85a4ae
MD5 (V01.03.0400_Mavic_dji_system.bin) = a5ac037462b4f902bfa6cb8d9fe395ae
MD5 (V01.03.0400_RC_Mavic_dji_system.bin) = d5f40b9231786d6d5053539a78a105c5
MD5 (V01.03.0500_Mavic_dji_system.bin) = 2934111740e9cec3cd65029754b71fd8
MD5 (V01.03.0509_P4P_dji_system.bin) = 93a1663f6675a813ed494e260bb54e89
MD5 (V01.03.0550_Mavic_dji_system.bin) = 34bdb52c8b8b7468f6312a5febf1838d
MD5 (V01.03.0550_RC_Mavic_dji_system.bin) = 06cc62f5d658c7461c758f3903b56c2a
MD5 (V01.03.0600_Mavic_dji_system.bin) = f3a40d447c39bf8e946f2b5a087dccd6
MD5 (V01.03.0600_RC_Mavic_dji_system.bin) = 06b7657e1c8a42faf4b6f847eefcb438
MD5 (V01.03.0700_Goggles_dji_system-2.bin) = 76eefdb955bfa416e2f43f2ac9f86b84
MD5 (V01.03.0700_Goggles_dji_system.bin) = 47e7ea9eb5f5609bbd8141f7edb3516c
MD5 (V01.03.0700_Mavic_dji_system.bin) = 891904fad23add85e8c50a7902f272df
MD5 (V01.03.0700_RC_Mavic_dji_system.bin) = 8c11d7e04c03142a50cc0c9538d49fa6
MD5 (V01.03.0800_Goggles_dji_system.bin) = e2c93ded968c148f94c7a81776ce1dfd
MD5 (V01.03.0800_Mavic_dji_system.bin) = 6602c26ed0729581246853d7c988a4ae
MD5 (V01.03.0800_RC_Mavic_dji_system.bin) = e2508fbf87ce87c0dc7fb7721e555901
MD5 (V01.03.0900_Goggles_dji_system.bin) = 1f82d27681217b4c388a593e4ba6f875
MD5 (V01.03.0900_Mavic_dji_system.bin) = 984446beb028443670091e07d3bbd752
MD5 (V01.03.0900_RC_Mavic_dji_system.bin) = beb6c9dea2a0ad5f688ada4d439e969f
MD5 (V01.04.0602_P4P_dji_system.bin) = 2a6b5baba26aa3203ecdc5450ba0473f
MD5 (V01.04.0602_P4P_dji_system.bin) = 46d325fafd60086add4c4c77c15132f7

MD5 (V02.00.0106_P4_dji_system.bin) = a49944bb254354ec064bee13c491fa1e
MD5 (data_copy.bin) = 133d14108497decbb85d79196ce703ca
MD5 (mavic_combined_400_root.bin) = 86b322026612e96fa09373bc8560674a
MD5 (mavic_combined_700_root.bin) = 3df0890c5e5a59ea1ef2476c4b728206

```
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

For more information on GPL rights as a DJI Enterprise end user see below:
![GPL Violation](https://pbs.twimg.com/media/DE1Bq2EUMAUbaQQ.jpg)

![GPL Violation](https://pbs.twimg.com/media/DE0nLtvUIAEElqv.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE0jqs3UMAEqaKl.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE0kC3uUIAEspBe.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE0kOyBWsAAU9eN.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE0jqtmUMAEtA3E.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE0kjvkUMAECMv3.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE0lrf5VoAAN9tq.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE0mAIEUQAEfsv5.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE0mcDuUIAE4Wug.jpg)
![GPL Violation](https://pbs.twimg.com/media/DE0nlY5VYAAZS58.jpg)

Never mind the fact that we are *seemingly* being forced into certain firmware variants as a *reaction* to CopterSafe NFZ bypass.

![You do not have to update the firmware and app if you don't want to](https://pbs.twimg.com/media/DE5s4L6VwAAzcKL.jpg)

![You do not have to update the firmware and app if you don't want to](https://pbs.twimg.com/media/DEVX8wyXgAAM8ox.jpg)

https://www.dji.com/newsroom/news/dji-updates-process-for-activating-software-and-firmware-updates
```
DJI Updates Process For Activating Software And Firmware Updates New Procedure Requires Login After Update; Password Reset Available
```

```
If this activation process is not performed, the aircraft will not have access to the correct geospatial information and flight functions for that region, 
and its operations will be restricted if you update the upcoming firmware: Live camera streaming will be disabled, and flight will be limited to a 50-meter 
(164-foot) radius up to 30 meters (98 feet) high.

The feature applies to all aircraft (mentioned above) that have been upgraded to the latest firmware or when using future versions of the DJI GO and GO 4 apps.
```

For posterity a bit of info on data_copy.bin aka the NFZ db abused by RedHerring

MD5 (data_copy.bin) = 133d14108497decbb85d79196ce703ca # example of an NFZ update 
```
$ ~/dji_research/tools/image.py nfz.sig 
{   'auth_key': b'GFAK',
    'blocks_cnt': 1,
    'enc_key': b'IAEK',
    'header_size': 224,
    'image_name': b'geof'
                  b'ense',
    'magic': b'IM*H',
    'payload_size': 2928640,
    'rsa_sig_size': 256,
    'scramble_key': <__main__.c_ubyte_Array_16 object at 0x10612f598>,
    'sha256_payload': <__main__.c_ubyte_Array_32 object at 0x10612f620>,
    'version': 1}
Can't find enc_key IAEK
Unpacking block {   'attrib': 1,
    'name': b'GFDB',
    'output_size': 2928640,
    'start_offset': 0}

$ file nfz.db 
nfz.db: SQLite 3.x database

$ sqlite3 nfz.db .schema
CREATE TABLE airmap_geofence_polygons (
        area_id int,
        points  blob,
        country int,
        lat     int,
        lng     int,
        radius  int,
        shape  int,
        sub_area_id int,
        height      int,
        area_level  int
      );
CREATE INDEX index_airmap_area_id on airmap_geofence_polygons (area_id);
CREATE INDEX index_airmap_lat_lng on airmap_geofence_polygons (lat, lng);
CREATE TABLE geofence_version (
        version            varchar(255),
        data_timestamp        int,
        area_count         int,
        remark varchar(255) DEFAULT NULL

      );

```


