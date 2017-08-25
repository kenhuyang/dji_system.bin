# dji_system.bin
Update:
DJI has made direct steps toward woking to GPL comliance: http://www.dji.com/opensource
https://s3.amazonaws.com/dji-brandsite-document/opensource/busybox-1.25.1.tar.gz
https://s3.amazonaws.com/dji-brandsite-document/opensource/mmc_utils.tar.gz

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


