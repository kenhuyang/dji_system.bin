# dji_system.bin
WARNING! Use this repo at your own risk. You CAN brick your DJI product if you don't know what you are doing.  
The author is not responsible for direct, indirect, incidental or consequential damages resulting from any defect, error or failure of this code repository to perform.

DJI is currently in violation of GPL... these binaries are intended to be distributed to end users that have purchased either an Inspire2, Goggles, Mavic, Spark, or P4 variant drone,and are seeking to downgrade their aircraft back to its factory state. 

If you are just here to learn how dji_system.bin is used for firmware downgrades please go here: https://github.com/MAVProxyUser/dji_system.bin/blob/master/HOWTO.md

NFZ databases's are one item that can be pushed in down/upgrade files, more detail on them can be found here: https://github.com/MAVProxyUser/dji_system.bin/blob/master/NFZ.md

GPL Update:
On Jul 18, 2017, at 10:30 AM, Bruce Perens wrote:
"Thank you (and whoever else helped) very much for the detailed examination which I see on your GIT repository. 
Please inform the DJI community that this morning I have written to DJI legal regarding the problem. I will inform you if they respond"

For information on the GPL violation issue please see: https://github.com/MAVProxyUser/dji_system.bin/blob/master/GPL.md

The heads of The Five Families of DJI Jailbreaking scene have met...
<img src=https://pbs.twimg.com/media/DFrZ-F1VwAAY9js.jpg>           

https://genius.com/Francis-ford-coppola-the-godfather-scene-8-annotated

Drone Corleone: "When...when did I ever refuse an accommodation? All of you know me here. When did I ever refuse? Except one time. And why? Because I believe this unlocked drone business is gonna destroy us in the years to come. I mean, it's not like ratemode, FPV or even, BLVOS which is something that most people want nowadays, and is forbidden to them... Even the police departments that've helped us in the past with gambling and other things are gonna refuse to help us when in comes to unlocked drones. And I believed that then and I believe that now."

bin4ry: "Times have changed. It's not like the Old Days when we can do anything we want."

Hostile: "I also don't believe in unlocked drones. For years I paid my people extra so they wouldn't do that kind of business. Somebody comes to them and says, "I have CopterSafe; if you put up three, four thousand dollar investment we can make fifty thousand distributing." So they can't resist. I want to control it as a business, to keep it respectable. *as he slams his hand on the table* I don't want it near warzones. I don't want it sold to militants! That's an infamia. In my city, we would keep the traffic in the Band chat – the Facebook users. They're animals anyway, so let them lose their souls..."

Drone Corleone: "I hoped that we would come here and reason together. And as a reasonable man I'm willing to do whatever's necessary to find a peaceful solution to these problems..."

bin4ry: "Then we are agreed. The traffic in unlocked drones will be permitted, but controlled and Drone Corleone will give up protection of the NFZ, and there will be the peace."

Drone Corleone: "I will not be the one to break the peace that we have made here today... "

### #DeejayeyeHackingClub information repos aka "The OG's" (Original Gangsters)
http://dji.retroroms.info/ - "Wiki"

https://github.com/fvantienen/dji_rev - This repository contains tools for reverse engineering DJI product firmware images.

https://github.com/Bin4ry/deejayeye-modder - APK "tweaks" for settings & "mods" for additional / altered functionality

https://github.com/hdnes/pyduml - Assistant-less firmware pushes and DUMLHacks referred to as DUMBHerring when used with "fireworks.tar" from RedHerring. DJI silently changes Assistant? great... we will just stop using it.

https://github.com/MAVProxyUser/P0VsRedHerring - RedHerring, aka "July 4th Independence Day exploit", "FTPD directory transversal 0day", etc. (Requires Assistant). We all needed a *public* root exploit... why not burn some 0day?

https://github.com/MAVProxyUser/dji_system.bin - Current Archive of dji_system.bin files that compose firmware updates referenced by MD5 sum. These can be used to upgrade and downgrade, and root your I2, P4, Mavic, Spark, Goggles, and Mavic RC to your hearts content. (Use with pyduml or DUMLDore)

https://github.com/MAVProxyUser/firm_cache - Extracted contents of dji_system.bin, in the future will be used to mix and match pieces of firmware for custom upgrade files. This repo was previously private... it is now open.

https://github.com/MAVProxyUser/DUMLrub - Ruby port of PyDUML, and firmware cherry picking tool. Allows rolling of custom firmware images.  

https://github.com/jezzab/DUMLdore - Even windows users need some love, so DUMLDore was created to help archive, and flash dji_system.bin files on windows platforms.

https://github.com/MAVProxyUser/DJI_ftpd_aes_unscramble - DJI has modified the GPL Busybox ftpd on Mavic, Spark, & Inspire 2 to include AES scrambling of downloaded files... this tool will reverse the scrambling
