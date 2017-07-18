place holder... put user supplied mods here. Please send PR to add to this folder. 
https://github.com/MAVProxyUser/dji_system.bin/compare

Dropbear adds sshd capability.  This tarfile contains a patchfile for /system/bin/start_dji_system.sh, which 
must be run to make this work. The patchfile is installed into /data/misc. The default is to make the root
password ( and all users for that matter ) RedHerringDerp. 
dropbear 4eb77862d76c2009860cde6b430adc91

Nano adds the 'nano' editor.  You need to set TERM=linux, and TERMINFO=/system/etc/terminfo
nano 02a9b3efbc256fd2370585c14bdc8976
