# dji_system.bin
DJI is currently in violation of GPL... these binaries are intended to be distributed to end users that have purchased either an inspire2, Mavic, Spark, or P4 variant drone,and are seeking to downgrade their aircraft back to its factory state. 

Never mind the fact that we are *seemingly* being forced into certain firmware variants as a *reaction* to CopterSafe NFZ bypass.

![You do not have to update the firmware and app if you don't want to](https://pbs.twimg.com/media/DE5s4L6VwAAzcKL.jpg)

Now...
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
MD5 (UniversalFireworksTar_dji_system.bin) = 10e4b4ba3da6e2e2455f2958ea897e9c
MD5 (V01.00.0300_Spark_dji_system.bin) = bf81af1c10318e8549bb78b0fef85013
MD5 (V01.00.0400_Spark_dji_system.bin) = 65f15f4cbe7d761459c7a09ebc660801 # (pulled from adiru aka troll: mossad911 VM)
MD5 (V01.03.0400_Mavic_dji_system.bin) = a5ac037462b4f902bfa6cb8d9fe395ae
MD5 (V01.03.0400_RC_Mavic_dji_system.bin) = d5f40b9231786d6d5053539a78a105c5 # (pulled from adiru aka troll: mossad911 VM)
MD5 (V01.03.0700_Mavic_dji_system.bin) = 891904fad23add85e8c50a7902f272df
MD5 (V01.03.0700_RC_Mavic_dji_system.bin) = 8c11d7e04c03142a50cc0c9538d49fa6
MD5 (V01.03.0800_Goggles_dji_system.bin) = e2c93ded968c148f94c7a81776ce1dfd
MD5 (V01.03.0800_Mavic_dji_system.bin) = 6602c26ed0729581246853d7c988a4ae
MD5 (V01.03.0900_Mavic_dji_system.bin) = 984446beb028443670091e07d3bbd752
MD5 (V01.01.0010_I2_dji_system.bin) = 7d04f199bd872c9372fdebddbef3c404
```

Known files from *homebrew* variants
```
MD5 (mavic_combined_400_root.bin) = 86b322026612e96fa09373bc8560674a - from hostile (drops root & downgrades to Mavic .400)
MD5 (mavic_combined_700_root.bin) = 3df0890c5e5a59ea1ef2476c4b728206 - *same* for .700
MD5 (V01.02.0602_P4crafted_dji_system.bin) = 36e11566ae6e303ec5c407f9c0f6c382
MD5 (V02.00.0106_P4crafted_dji_system.bin) = a49944bb254354ec064bee13c491fa1e
MD5 (V01.03.0700_Gogglescrafted.1.03.0700.bin) = 76eefdb955bfa416e2f43f2ac9f86b84
MD5 (V01.00.0330_I2crafted_dji_system.bin) = 0a5c437812b91355c9ae0d4d28d505d1
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
