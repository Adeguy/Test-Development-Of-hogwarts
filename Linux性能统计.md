#### [ck281183@shell.ceshiren.com ~]$ ll
total 0
#### [ck281183@shell.ceshiren.com ~]$ pwd
/home/ck281183
#### [ck281183@shell.ceshiren.com ~]$ mkdir newfile
#### [ck281183@shell.ceshiren.com ~]$ ll
total 4
drwxrwxr-x 2 ck281183 ck281183 4096 Nov 28 16:18 newfile
#### [ck281183@shell.ceshiren.com ~]$ cd newfile/
#### [ck281183@shell.ceshiren.com newfile]$ touch newtext.txt
#### [ck281183@shell.ceshiren.com newfile]$ ll
total 0
-rw-rw-r-- 1 ck281183 ck281183 0 Nov 28 16:20 newtext.txt
#### [ck281183@shell.ceshiren.com newfile]$ echo 123 >newtext.txt 
#### [ck281183@shell.ceshiren.com newfile]$ cat newtext.txt 
123
#### [ck281183@shell.ceshiren.com newfile]$ echo 123234 >>newtext.txt 
#### [ck281183@shell.ceshiren.com newfile]$ cat newtext.txt 
123
123234
#### [ck281183@shell.ceshiren.com newfile]$ vim newtext.txt 
#### [ck281183@shell.ceshiren.com newfile]$ cat newtext.txt 
123
123
123456
#### [ck281183@shell.ceshiren.com newfile]$ chmod 755 newtext.txt 
#### [ck281183@shell.ceshiren.com newfile]$ ll
total 4
-rwxr-xr-x 1 ck281183 ck281183 15 Nov 28 16:29 newtext.txt
#### [root@wxgdfwq-01 soft]# top
top - 00:06:59 up 10:06,  1 user,  load average: 0.00, 0.03, 0.05
Tasks: 157 total,   1 running, 156 sleeping,   0 stopped,   0 zombie
%Cpu(s):  0.0 us,  0.0 sy,  0.0 ni,100.0 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
KiB Mem :   995636 total,    96004 free,   473092 used,   426540 buff/cache
KiB Swap:  1048572 total,  1048572 free,        0 used.   338684 avail Mem 

   PID USER      PR  NI    VIRT    RES    SHR S %CPU %MEM     TIME+ COMMAND                                          
 11559 root      20   0  162100   2308   1588 R  0.3  0.2   0:00.03 top                                              
     1 root      20   0  126128   4568   2620 S  0.0  0.5   0:01.40 systemd                                          
     2 root      20   0       0      0      0 S  0.0  0.0   0:00.00 kthreadd                                         
     4 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 kworker/0:0H                                     
     6 root      20   0       0      0      0 S  0.0  0.0   0:00.40 ksoftirqd/0                                      
     7 root      rt   0       0      0      0 S  0.0  0.0   0:00.00 migration/0                                      
     8 root      20   0       0      0      0 S  0.0  0.0   0:00.00 rcu_bh                                           
     9 root      20   0       0      0      0 S  0.0  0.0   0:00.51 rcu_sched                                        
    10 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 lru-add-drain                                    
    11 root      rt   0       0      0      0 S  0.0  0.0   0:00.22 watchdog/0                                       
    13 root      20   0       0      0      0 S  0.0  0.0   0:00.00 kdevtmpfs                                        
    14 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 netns                                            
    15 root      20   0       0      0      0 S  0.0  0.0   0:00.01 khungtaskd                                       
    16 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 writeback                                        
    17 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 kintegrityd                                      
    18 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 bioset                                           
    19 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 bioset                                           
    20 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 bioset                                           
    21 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 kblockd                                          
    22 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 md                                               
    23 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 edac-poller                                      
    24 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 watchdogd                                        
    30 root      20   0       0      0      0 S  0.0  0.0   0:00.00 kswapd0                                          
    31 root      25   5       0      0      0 S  0.0  0.0   0:00.00 ksmd                                             
    32 root      39  19       0      0      0 S  0.0  0.0   0:00.27 khugepaged                                       
    33 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 crypto                                           
    41 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 kthrotld                                         
    43 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 kmpath_rdacd                                     
    44 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 kaluad                                           
    45 root       0 -20       0      0      0 S  0.0  0.0   0:00.00 kpsmoused                                        
#### [root@wxgdfwq-01 soft]# uptime
 00:07:25 up 10:07,  1 user,  load average: 0.00, 0.02, 0.05
#### [root@wxgdfwq-01 soft]# ps aux 
USER        PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root          1  0.0  0.4 126128  4568 ?        Ss   11月28   0:01 /usr/lib/systemd/systemd --switched-root --system 
root          2  0.0  0.0      0     0 ?        S    11月28   0:00 [kthreadd]
root          4  0.0  0.0      0     0 ?        S<   11月28   0:00 [kworker/0:0H]
root          6  0.0  0.0      0     0 ?        S    11月28   0:00 [ksoftirqd/0]
root          7  0.0  0.0      0     0 ?        S    11月28   0:00 [migration/0]
root          8  0.0  0.0      0     0 ?        S    11月28   0:00 [rcu_bh]
root          9  0.0  0.0      0     0 ?        S    11月28   0:00 [rcu_sched]
root         10  0.0  0.0      0     0 ?        S<   11月28   0:00 [lru-add-drain]
root         11  0.0  0.0      0     0 ?        S    11月28   0:00 [watchdog/0]
root         13  0.0  0.0      0     0 ?        S    11月28   0:00 [kdevtmpfs]
root         14  0.0  0.0      0     0 ?        S<   11月28   0:00 [netns]
root         15  0.0  0.0      0     0 ?        S    11月28   0:00 [khungtaskd]
root         16  0.0  0.0      0     0 ?        S<   11月28   0:00 [writeback]
root         17  0.0  0.0      0     0 ?        S<   11月28   0:00 [kintegrityd]
root         18  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root         19  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root         20  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root         21  0.0  0.0      0     0 ?        S<   11月28   0:00 [kblockd]
root         22  0.0  0.0      0     0 ?        S<   11月28   0:00 [md]
root         23  0.0  0.0      0     0 ?        S<   11月28   0:00 [edac-poller]
root         24  0.0  0.0      0     0 ?        S<   11月28   0:00 [watchdogd]
root         30  0.0  0.0      0     0 ?        S    11月28   0:00 [kswapd0]
root         31  0.0  0.0      0     0 ?        SN   11月28   0:00 [ksmd]
root         32  0.0  0.0      0     0 ?        SN   11月28   0:00 [khugepaged]
root         33  0.0  0.0      0     0 ?        S<   11月28   0:00 [crypto]
root         41  0.0  0.0      0     0 ?        S<   11月28   0:00 [kthrotld]
root         43  0.0  0.0      0     0 ?        S<   11月28   0:00 [kmpath_rdacd]
root         44  0.0  0.0      0     0 ?        S<   11月28   0:00 [kaluad]
root         45  0.0  0.0      0     0 ?        S<   11月28   0:00 [kpsmoused]
root         47  0.0  0.0      0     0 ?        S<   11月28   0:00 [ipv6_addrconf]
root         60  0.0  0.0      0     0 ?        S<   11月28   0:00 [deferwq]
root         96  0.0  0.0      0     0 ?        S    11月28   0:00 [kauditd]
root        271  0.0  0.0      0     0 ?        S<   11月28   0:00 [nfit]
root        275  0.0  0.0      0     0 ?        S<   11月28   0:00 [mpt_poll_0]
root        277  0.0  0.0      0     0 ?        S<   11月28   0:00 [mpt/0]
root        278  0.0  0.0      0     0 ?        S<   11月28   0:00 [ata_sff]
root        289  0.0  0.0      0     0 ?        S    11月28   0:00 [scsi_eh_0]
root        290  0.0  0.0      0     0 ?        S<   11月28   0:00 [scsi_tmf_0]
root        291  0.0  0.0      0     0 ?        S    11月28   0:00 [scsi_eh_1]
root        292  0.0  0.0      0     0 ?        S    11月28   0:00 [kworker/u256:2]
root        294  0.0  0.0      0     0 ?        S<   11月28   0:00 [scsi_tmf_1]
root        296  0.0  0.0      0     0 ?        S    11月28   0:00 [scsi_eh_2]
root        298  0.0  0.0      0     0 ?        S<   11月28   0:00 [scsi_tmf_2]
root        365  0.0  0.0      0     0 ?        S<   11月28   0:00 [kdmflush]
root        366  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root        376  0.0  0.0      0     0 ?        S<   11月28   0:00 [kdmflush]
root        377  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root        389  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root        390  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfsalloc]
root        391  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs_mru_cache]
root        392  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-buf/dm-0]
root        393  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-data/dm-0]
root        394  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-conv/dm-0]
root        395  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-cil/dm-0]
root        396  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-reclaim/dm-]
root        397  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-log/dm-0]
root        398  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-eofblocks/d]
root        399  0.0  0.0      0     0 ?        S    11月28   0:01 [xfsaild/dm-0]
root        400  0.0  0.0      0     0 ?        S<   11月28   0:00 [kworker/0:1H]
root        488  0.0  0.3  37336  3644 ?        Ss   11月28   0:00 /usr/lib/systemd/systemd-journald
root        509  0.0  0.1 190376  1352 ?        Ss   11月28   0:00 /usr/sbin/lvmetad -f
root        520  0.0  0.2  46496  2832 ?        Ss   11月28   0:00 /usr/lib/systemd/systemd-udevd
root        710  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-buf/sda1]
root        715  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-data/sda1]
root        717  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-conv/sda1]
root        719  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-cil/sda1]
root        721  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-reclaim/sda]
root        726  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-log/sda1]
root        730  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-eofblocks/s]
root        733  0.0  0.0      0     0 ?        S    11月28   0:00 [xfsaild/sda1]
root       1049  0.0  0.0      0     0 ?        S<   11月28   0:00 [rpciod]
root       1050  0.0  0.0      0     0 ?        S<   11月28   0:00 [xprtiod]
root       1052  0.0  0.0  55532   856 ?        S<sl 11月28   0:00 /sbin/auditd
root       1054  0.0  0.0  84556   916 ?        S<sl 11月28   0:00 /sbin/audispd
root       1056  0.0  0.1  55620  1424 ?        S<   11月28   0:00 /usr/sbin/sedispatch
root       1077  0.0  0.7 430624  7544 ?        Ssl  11月28   0:00 /usr/sbin/ModemManager
rtkit      1078  0.0  0.1 198784  1800 ?        SNsl 11月28   0:00 /usr/libexec/rtkit-daemon
root       1079  0.0  0.5 168304  5196 ?        Ss   11月28   0:00 /usr/bin/VGAuthService -s
root       1080  0.0  0.5 293528  5248 ?        Ssl  11月28   0:38 /usr/bin/vmtoolsd
libstor+   1085  0.0  0.0   8580   824 ?        Ss   11月28   0:00 /usr/bin/lsmd -d
rpc        1087  0.0  0.1  69256  1004 ?        Ss   11月28   0:00 /sbin/rpcbind -w
root       1089  0.0  0.1  16900  1388 ?        SNs  11月28   0:00 /usr/sbin/alsactl -s -n 19 -c -E ALSA_CONFIG_PATH=
avahi      1093  0.0  0.2  62272  2080 ?        Ss   11月28   0:00 avahi-daemon: running [wxgdfwq-01.local]
root       1097  0.0  0.4 396680  4260 ?        Ssl  11月28   0:00 /usr/libexec/accounts-daemon
root       1104  0.0  0.3  90652  3228 ?        Ss   11月28   0:01 /sbin/rngd -f
root       1107  0.0  0.6 228484  6040 ?        Ss   11月28   0:00 /usr/sbin/abrtd -d -s
chrony     1108  0.0  0.1 117808  1828 ?        S    11月28   0:00 /usr/sbin/chronyd
root       1112  0.0  0.4 225960  4928 ?        Ss   11月28   0:00 /usr/bin/abrt-watch-log -F BUG: WARNING: at WARNIN
avahi      1114  0.0  0.0  62140   404 ?        S    11月28   0:00 avahi-daemon: chroot helper
root       1115  0.0  0.4 225960  4920 ?        Ss   11月28   0:00 /usr/bin/abrt-watch-log -F Backtrace /var/log/Xorg
dbus       1116  0.0  0.3  61536  3428 ?        Ss   11月28   0:00 /usr/bin/dbus-daemon --system --address=systemd: -
root       1136  0.0  1.1 479536 11460 ?        Ssl  11月28   0:01 /usr/sbin/NetworkManager --no-daemon
root       1137  0.0  0.2  52852  2804 ?        Ss   11月28   0:00 /usr/sbin/smartd -n -q never
polkitd    1138  0.0  1.3 616688 13104 ?        Ssl  11月28   0:06 /usr/lib/polkit-1/polkitd --no-debug
root       1139  0.0  0.6 451328  6460 ?        Ssl  11月28   0:00 /usr/libexec/udisks2/udisksd
root       1144  0.0  0.1  26384  1792 ?        Ss   11月28   0:00 /usr/lib/systemd/systemd-logind
root       1150  0.0  0.1 201428  1280 ?        Ssl  11月28   0:00 /usr/sbin/gssproxy -D
root       1175  0.0  0.0 115408   968 ?        S    11月28   0:00 /bin/bash /usr/sbin/ksmtuned
root       1547  0.0  0.4 198072  4292 ?        Ss   11月28   0:00 /usr/sbin/cupsd -f
root       1548  0.0  1.7 574524 17572 ?        Ssl  11月28   0:05 /usr/bin/python2 -Es /usr/sbin/tuned -l -P
root       1549  0.0  0.4 112984  4320 ?        Ss   11月28   0:00 /usr/sbin/sshd -D
root       1551  0.0  0.5 218640  5272 ?        Ssl  11月28   0:02 /usr/sbin/rsyslogd -n
root       1554  0.0  1.5 1011696 15712 ?       Ssl  11月28   0:00 /usr/sbin/libvirtd
root       1562  0.0  0.1 126384  1624 ?        Ss   11月28   0:00 /usr/sbin/crond -n
root       1566  0.0  0.0  25908   952 ?        Ss   11月28   0:00 /usr/sbin/atd -f
root       1567  0.0  0.4 481560  4824 ?        Ssl  11月28   0:00 /usr/sbin/gdm
root       1585  0.0  3.0 424516 30260 tty1     Ssl+ 11月28   0:00 /usr/bin/X :0 -background none -noreset -audit 4 -
nobody     1802  0.0  0.1  56124  1136 ?        S    11月28   0:00 /usr/sbin/dnsmasq --conf-file=/var/lib/libvirt/dns
root       1805  0.0  0.0  56096   392 ?        S    11月28   0:00 /usr/sbin/dnsmasq --conf-file=/var/lib/libvirt/dns
root       1838  0.0  0.2  91872  2272 ?        Ss   11月28   0:00 /usr/libexec/postfix/master -w
postfix    1849  0.0  0.4  92152  4132 ?        S    11月28   0:00 qmgr -l -t unix -u
root       1978  0.0  0.4 363240  4884 ?        Sl   11月28   0:00 gdm-session-worker [pam/gdm-launch-environment]
gdm        1996  0.0  1.1 671536 11172 ?        Ssl  11月28   0:00 /usr/libexec/gnome-session-binary --autostart /usr
gdm        2007  0.0  0.0  59016   976 ?        S    11月28   0:00 dbus-launch --exit-with-session /usr/libexec/gnome
gdm        2013  0.0  0.1  60492  1888 ?        Ss   11月28   0:00 /usr/bin/dbus-daemon --fork --print-pid 5 --print-
gdm        2020  0.0  0.3 346840  3672 ?        Sl   11月28   0:00 /usr/libexec/at-spi-bus-launcher
gdm        2025  0.0  0.2  60064  2296 ?        S    11月28   0:00 /usr/bin/dbus-daemon --config-file=/usr/share/defa
gdm        2028  0.0  0.3 233104  3960 ?        Sl   11月28   0:00 /usr/libexec/at-spi2-registryd --use-gnome-session
gdm        2049  0.0 13.8 2945656 138104 ?      Sl   11月28   0:13 /usr/bin/gnome-shell
root       2056  0.0  0.7 430484  7324 ?        Ssl  11月28   0:00 /usr/libexec/upowerd
gdm        2071  0.0  0.6 1252312 6400 ?        S<l  11月28   0:00 /usr/bin/pulseaudio --start --log-target=syslog
gdm        2088  0.0  0.5 527052  5520 ?        Sl   11月28   0:00 ibus-daemon --xim --panel disable
gdm        2091  0.0  0.5 376172  5636 ?        Sl   11月28   0:00 /usr/libexec/ibus-dconf
gdm        2094  0.0  1.4 465356 14040 ?        Sl   11月28   0:00 /usr/libexec/ibus-x11 --kill-daemon
gdm        2098  0.0  0.3 376152  3468 ?        Sl   11月28   0:00 /usr/libexec/ibus-portal
gdm        2108  0.0  0.2 364920  2904 ?        Sl   11月28   0:00 /usr/libexec/xdg-permission-store
root       2117  0.0  0.4 398900  4148 ?        Ssl  11月28   0:00 /usr/libexec/boltd
root       2123  0.0  0.5 410768  5496 ?        Ssl  11月28   0:00 /usr/libexec/packagekitd
root       2128  0.0  0.3  78660  3368 ?        Ss   11月28   0:00 /usr/sbin/wpa_supplicant -u -f /var/log/wpa_suppli
gdm        2131  0.0  1.5 615788 15376 ?        Sl   11月28   0:00 /usr/libexec/gsd-xsettings
gdm        2133  0.0  0.3 376760  3444 ?        Sl   11月28   0:00 /usr/libexec/gsd-a11y-settings
gdm        2136  0.0  1.3 465040 13808 ?        Sl   11月28   0:00 /usr/libexec/gsd-clipboard
gdm        2140  0.0  1.5 714704 14976 ?        Sl   11月28   0:05 /usr/libexec/gsd-color
gdm        2141  0.0  0.8 465660  8020 ?        Sl   11月28   0:00 /usr/libexec/gsd-datetime
gdm        2145  0.0  0.3 380888  3040 ?        Sl   11月28   0:00 /usr/libexec/gsd-housekeeping
gdm        2147  0.0  1.4 614808 14076 ?        Sl   11月28   0:00 /usr/libexec/gsd-keyboard
gdm        2152  0.0  1.6 1012672 16108 ?       Sl   11月28   0:00 /usr/libexec/gsd-media-keys
gdm        2157  0.0  0.2 300624  2896 ?        Sl   11月28   0:00 /usr/libexec/gsd-mouse
gdm        2163  0.0  1.7 632348 17088 ?        Sl   11月28   0:00 /usr/libexec/gsd-power
gdm        2167  0.0  0.4 363352  4576 ?        Sl   11月28   0:00 /usr/libexec/gsd-print-notifications
gdm        2169  0.0  0.3 317852  3140 ?        Sl   11月28   0:00 /usr/libexec/gsd-rfkill
gdm        2176  0.0  0.3 374360  3068 ?        Sl   11月28   0:00 /usr/libexec/gsd-screensaver-proxy
gdm        2181  0.0  0.4 411848  4376 ?        Sl   11月28   0:00 /usr/libexec/gsd-sharing
gdm        2186  0.0  0.5 472804  5260 ?        Sl   11月28   0:00 /usr/libexec/gsd-smartcard
gdm        2189  0.0  0.4 455260  4940 ?        Sl   11月28   0:00 /usr/libexec/gsd-sound
gdm        2193  0.0  1.6 623604 16628 ?        Sl   11月28   0:00 /usr/libexec/gsd-wacom
colord     2214  0.0  0.6 419772  6396 ?        Ssl  11月28   0:00 /usr/libexec/colord
root       2227  0.0  0.6 163888  6144 ?        Ss   11月28   0:00 sshd: root@pts/0
gdm        2235  0.0  0.3 302356  3416 ?        Sl   11月28   0:00 /usr/libexec/ibus-engine-simple
root       2247  0.0  0.3 117084  3700 pts/0    Ss   11月28   0:00 -bash
root       9764  0.0  0.0      0     0 ?        S    11月28   0:00 [kworker/u256:1]
postfix   11487  0.0  0.4  91976  4116 ?        S    00:00   0:00 pickup -l -t unix -u
root      12232  0.0  0.0      0     0 ?        S    01:15   0:00 [kworker/0:2]
root      12241  0.0  0.0      0     0 ?        R    01:16   0:00 [kworker/0:3]
root      12294  0.0  0.0      0     0 ?        S    01:21   0:00 [kworker/0:0]
root      12334  0.0  0.0 108052   360 ?        S    01:26   0:00 sleep 60
root      12336  0.0  0.1 155448  1876 pts/0    R+   01:27   0:00 ps aux
#### [root@wxgdfwq-01 soft]# free -m > memory_used.txt
#### [root@wxgdfwq-01 soft]# ll
总用量 8
-rw-r--r-- 1 root root 204 11月 29 01:29 memory_used.txt
-rw-r--r-- 1 root root  39 11月 28 22:13 test.txt
#### [root@wxgdfwq-01 soft]# wc -c memory_used.txt 
204 memory_used.txt
#### [root@wxgdfwq-01 soft]# cat memory_used.txt | wc -c
204
#### [root@wxgdfwq-01 soft]# sort -r -u -b memory_used.txt > sorted_memory_used.txt
#### [root@wxgdfwq-01 soft]# ps aux
USER        PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root          1  0.0  0.4 126128  4568 ?        Ss   11月28   0:01 /usr/lib/systemd/systemd --switched-root --system 
root          2  0.0  0.0      0     0 ?        S    11月28   0:00 [kthreadd]
root          4  0.0  0.0      0     0 ?        S<   11月28   0:00 [kworker/0:0H]
root          6  0.0  0.0      0     0 ?        S    11月28   0:00 [ksoftirqd/0]
root          7  0.0  0.0      0     0 ?        S    11月28   0:00 [migration/0]
root          8  0.0  0.0      0     0 ?        S    11月28   0:00 [rcu_bh]
root          9  0.0  0.0      0     0 ?        S    11月28   0:00 [rcu_sched]
root         10  0.0  0.0      0     0 ?        S<   11月28   0:00 [lru-add-drain]
root         11  0.0  0.0      0     0 ?        S    11月28   0:00 [watchdog/0]
root         13  0.0  0.0      0     0 ?        S    11月28   0:00 [kdevtmpfs]
root         14  0.0  0.0      0     0 ?        S<   11月28   0:00 [netns]
root         15  0.0  0.0      0     0 ?        S    11月28   0:00 [khungtaskd]
root         16  0.0  0.0      0     0 ?        S<   11月28   0:00 [writeback]
root         17  0.0  0.0      0     0 ?        S<   11月28   0:00 [kintegrityd]
root         18  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root         19  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root         20  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root         21  0.0  0.0      0     0 ?        S<   11月28   0:00 [kblockd]
root         22  0.0  0.0      0     0 ?        S<   11月28   0:00 [md]
root         23  0.0  0.0      0     0 ?        S<   11月28   0:00 [edac-poller]
root         24  0.0  0.0      0     0 ?        S<   11月28   0:00 [watchdogd]
root         30  0.0  0.0      0     0 ?        S    11月28   0:00 [kswapd0]
root         31  0.0  0.0      0     0 ?        SN   11月28   0:00 [ksmd]
root         32  0.0  0.0      0     0 ?        SN   11月28   0:00 [khugepaged]
root         33  0.0  0.0      0     0 ?        S<   11月28   0:00 [crypto]
root         41  0.0  0.0      0     0 ?        S<   11月28   0:00 [kthrotld]
root         43  0.0  0.0      0     0 ?        S<   11月28   0:00 [kmpath_rdacd]
root         44  0.0  0.0      0     0 ?        S<   11月28   0:00 [kaluad]
root         45  0.0  0.0      0     0 ?        S<   11月28   0:00 [kpsmoused]
root         47  0.0  0.0      0     0 ?        S<   11月28   0:00 [ipv6_addrconf]
root         60  0.0  0.0      0     0 ?        S<   11月28   0:00 [deferwq]
root         96  0.0  0.0      0     0 ?        S    11月28   0:00 [kauditd]
root        271  0.0  0.0      0     0 ?        S<   11月28   0:00 [nfit]
root        275  0.0  0.0      0     0 ?        S<   11月28   0:00 [mpt_poll_0]
root        277  0.0  0.0      0     0 ?        S<   11月28   0:00 [mpt/0]
root        278  0.0  0.0      0     0 ?        S<   11月28   0:00 [ata_sff]
root        289  0.0  0.0      0     0 ?        S    11月28   0:00 [scsi_eh_0]
root        290  0.0  0.0      0     0 ?        S<   11月28   0:00 [scsi_tmf_0]
root        291  0.0  0.0      0     0 ?        S    11月28   0:00 [scsi_eh_1]
root        292  0.0  0.0      0     0 ?        S    11月28   0:00 [kworker/u256:2]
root        294  0.0  0.0      0     0 ?        S<   11月28   0:00 [scsi_tmf_1]
root        296  0.0  0.0      0     0 ?        S    11月28   0:00 [scsi_eh_2]
root        298  0.0  0.0      0     0 ?        S<   11月28   0:00 [scsi_tmf_2]
root        365  0.0  0.0      0     0 ?        S<   11月28   0:00 [kdmflush]
root        366  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root        376  0.0  0.0      0     0 ?        S<   11月28   0:00 [kdmflush]
root        377  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root        389  0.0  0.0      0     0 ?        S<   11月28   0:00 [bioset]
root        390  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfsalloc]
root        391  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs_mru_cache]
root        392  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-buf/dm-0]
root        393  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-data/dm-0]
root        394  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-conv/dm-0]
root        395  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-cil/dm-0]
root        396  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-reclaim/dm-]
root        397  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-log/dm-0]
root        398  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-eofblocks/d]
root        399  0.0  0.0      0     0 ?        S    11月28   0:01 [xfsaild/dm-0]
root        400  0.0  0.0      0     0 ?        S<   11月28   0:00 [kworker/0:1H]
root        488  0.0  0.3  37336  3644 ?        Ss   11月28   0:00 /usr/lib/systemd/systemd-journald
root        509  0.0  0.1 190376  1352 ?        Ss   11月28   0:00 /usr/sbin/lvmetad -f
root        520  0.0  0.2  46496  2832 ?        Ss   11月28   0:00 /usr/lib/systemd/systemd-udevd
root        710  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-buf/sda1]
root        715  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-data/sda1]
root        717  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-conv/sda1]
root        719  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-cil/sda1]
root        721  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-reclaim/sda]
root        726  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-log/sda1]
root        730  0.0  0.0      0     0 ?        S<   11月28   0:00 [xfs-eofblocks/s]
root        733  0.0  0.0      0     0 ?        S    11月28   0:00 [xfsaild/sda1]
root       1049  0.0  0.0      0     0 ?        S<   11月28   0:00 [rpciod]
root       1050  0.0  0.0      0     0 ?        S<   11月28   0:00 [xprtiod]
root       1052  0.0  0.0  55532   856 ?        S<sl 11月28   0:00 /sbin/auditd
root       1054  0.0  0.0  84556   916 ?        S<sl 11月28   0:00 /sbin/audispd
root       1056  0.0  0.1  55620  1424 ?        S<   11月28   0:00 /usr/sbin/sedispatch
root       1077  0.0  0.7 430624  7544 ?        Ssl  11月28   0:00 /usr/sbin/ModemManager
rtkit      1078  0.0  0.1 198784  1800 ?        SNsl 11月28   0:00 /usr/libexec/rtkit-daemon
root       1079  0.0  0.5 168304  5196 ?        Ss   11月28   0:00 /usr/bin/VGAuthService -s
root       1080  0.0  0.5 293528  5248 ?        Ssl  11月28   0:39 /usr/bin/vmtoolsd
libstor+   1085  0.0  0.0   8580   824 ?        Ss   11月28   0:00 /usr/bin/lsmd -d
rpc        1087  0.0  0.1  69256  1004 ?        Ss   11月28   0:00 /sbin/rpcbind -w
root       1089  0.0  0.1  16900  1388 ?        SNs  11月28   0:00 /usr/sbin/alsactl -s -n 19 -c -E ALSA_CONFIG_PATH=
avahi      1093  0.0  0.2  62272  2080 ?        Ss   11月28   0:00 avahi-daemon: running [wxgdfwq-01.local]
root       1097  0.0  0.4 396680  4260 ?        Ssl  11月28   0:00 /usr/libexec/accounts-daemon
root       1104  0.0  0.3  90652  3228 ?        Ss   11月28   0:01 /sbin/rngd -f
root       1107  0.0  0.6 228484  6040 ?        Ss   11月28   0:00 /usr/sbin/abrtd -d -s
chrony     1108  0.0  0.1 117808  1828 ?        S    11月28   0:00 /usr/sbin/chronyd
root       1112  0.0  0.4 225960  4928 ?        Ss   11月28   0:00 /usr/bin/abrt-watch-log -F BUG: WARNING: at WARNIN
avahi      1114  0.0  0.0  62140   404 ?        S    11月28   0:00 avahi-daemon: chroot helper
root       1115  0.0  0.4 225960  4920 ?        Ss   11月28   0:00 /usr/bin/abrt-watch-log -F Backtrace /var/log/Xorg
dbus       1116  0.0  0.3  61536  3428 ?        Ss   11月28   0:00 /usr/bin/dbus-daemon --system --address=systemd: -
root       1136  0.0  1.1 479536 11460 ?        Ssl  11月28   0:01 /usr/sbin/NetworkManager --no-daemon
root       1137  0.0  0.2  52852  2804 ?        Ss   11月28   0:00 /usr/sbin/smartd -n -q never
polkitd    1138  0.0  1.3 616688 13112 ?        Ssl  11月28   0:06 /usr/lib/polkit-1/polkitd --no-debug
root       1139  0.0  0.6 451328  6460 ?        Ssl  11月28   0:00 /usr/libexec/udisks2/udisksd
root       1144  0.0  0.1  26384  1792 ?        Ss   11月28   0:00 /usr/lib/systemd/systemd-logind
root       1150  0.0  0.1 201428  1280 ?        Ssl  11月28   0:00 /usr/sbin/gssproxy -D
root       1175  0.0  0.0 115408   968 ?        S    11月28   0:00 /bin/bash /usr/sbin/ksmtuned
root       1547  0.0  0.4 198072  4292 ?        Ss   11月28   0:00 /usr/sbin/cupsd -f
root       1548  0.0  1.7 574524 17572 ?        Ssl  11月28   0:05 /usr/bin/python2 -Es /usr/sbin/tuned -l -P
root       1549  0.0  0.4 112984  4320 ?        Ss   11月28   0:00 /usr/sbin/sshd -D
root       1551  0.0  0.5 218640  5280 ?        Ssl  11月28   0:02 /usr/sbin/rsyslogd -n
root       1554  0.0  1.5 1011696 15712 ?       Ssl  11月28   0:00 /usr/sbin/libvirtd
root       1562  0.0  0.1 126384  1624 ?        Ss   11月28   0:00 /usr/sbin/crond -n
root       1566  0.0  0.0  25908   952 ?        Ss   11月28   0:00 /usr/sbin/atd -f
root       1567  0.0  0.4 481560  4824 ?        Ssl  11月28   0:00 /usr/sbin/gdm
root       1585  0.0  3.0 424516 30260 tty1     Ssl+ 11月28   0:00 /usr/bin/X :0 -background none -noreset -audit 4 -
nobody     1802  0.0  0.1  56124  1136 ?        S    11月28   0:00 /usr/sbin/dnsmasq --conf-file=/var/lib/libvirt/dns
root       1805  0.0  0.0  56096   392 ?        S    11月28   0:00 /usr/sbin/dnsmasq --conf-file=/var/lib/libvirt/dns
root       1838  0.0  0.2  91872  2272 ?        Ss   11月28   0:00 /usr/libexec/postfix/master -w
postfix    1849  0.0  0.4  92152  4132 ?        S    11月28   0:00 qmgr -l -t unix -u
root       1978  0.0  0.4 363240  4884 ?        Sl   11月28   0:00 gdm-session-worker [pam/gdm-launch-environment]
gdm        1996  0.0  1.1 671536 11172 ?        Ssl  11月28   0:00 /usr/libexec/gnome-session-binary --autostart /usr
gdm        2007  0.0  0.0  59016   976 ?        S    11月28   0:00 dbus-launch --exit-with-session /usr/libexec/gnome
gdm        2013  0.0  0.1  60492  1888 ?        Ss   11月28   0:00 /usr/bin/dbus-daemon --fork --print-pid 5 --print-
gdm        2020  0.0  0.3 346840  3672 ?        Sl   11月28   0:00 /usr/libexec/at-spi-bus-launcher
gdm        2025  0.0  0.2  60064  2296 ?        S    11月28   0:00 /usr/bin/dbus-daemon --config-file=/usr/share/defa
gdm        2028  0.0  0.3 233104  3960 ?        Sl   11月28   0:00 /usr/libexec/at-spi2-registryd --use-gnome-session
gdm        2049  0.0 13.8 2945656 138104 ?      Sl   11月28   0:13 /usr/bin/gnome-shell
root       2056  0.0  0.7 430484  7324 ?        Ssl  11月28   0:00 /usr/libexec/upowerd
gdm        2071  0.0  0.6 1252312 6400 ?        S<l  11月28   0:00 /usr/bin/pulseaudio --start --log-target=syslog
gdm        2088  0.0  0.5 527052  5520 ?        Sl   11月28   0:00 ibus-daemon --xim --panel disable
gdm        2091  0.0  0.5 376172  5636 ?        Sl   11月28   0:00 /usr/libexec/ibus-dconf
gdm        2094  0.0  1.4 465356 14040 ?        Sl   11月28   0:00 /usr/libexec/ibus-x11 --kill-daemon
gdm        2098  0.0  0.3 376152  3468 ?        Sl   11月28   0:00 /usr/libexec/ibus-portal
gdm        2108  0.0  0.2 364920  2904 ?        Sl   11月28   0:00 /usr/libexec/xdg-permission-store
root       2117  0.0  0.4 398900  4148 ?        Ssl  11月28   0:00 /usr/libexec/boltd
root       2123  0.0  0.5 410768  5496 ?        Ssl  11月28   0:00 /usr/libexec/packagekitd
root       2128  0.0  0.3  78660  3368 ?        Ss   11月28   0:00 /usr/sbin/wpa_supplicant -u -f /var/log/wpa_suppli
gdm        2131  0.0  1.5 615788 15376 ?        Sl   11月28   0:00 /usr/libexec/gsd-xsettings
gdm        2133  0.0  0.3 376760  3444 ?        Sl   11月28   0:00 /usr/libexec/gsd-a11y-settings
gdm        2136  0.0  1.3 465040 13808 ?        Sl   11月28   0:00 /usr/libexec/gsd-clipboard
gdm        2140  0.0  1.5 714704 14976 ?        Sl   11月28   0:05 /usr/libexec/gsd-color
gdm        2141  0.0  0.8 465660  8020 ?        Sl   11月28   0:00 /usr/libexec/gsd-datetime
gdm        2145  0.0  0.3 380888  3040 ?        Sl   11月28   0:00 /usr/libexec/gsd-housekeeping
gdm        2147  0.0  1.4 614808 14076 ?        Sl   11月28   0:00 /usr/libexec/gsd-keyboard
gdm        2152  0.0  1.6 1012672 16108 ?       Sl   11月28   0:00 /usr/libexec/gsd-media-keys
gdm        2157  0.0  0.2 300624  2896 ?        Sl   11月28   0:00 /usr/libexec/gsd-mouse
gdm        2163  0.0  1.7 632348 17088 ?        Sl   11月28   0:00 /usr/libexec/gsd-power
gdm        2167  0.0  0.4 363352  4576 ?        Sl   11月28   0:00 /usr/libexec/gsd-print-notifications
gdm        2169  0.0  0.3 317852  3140 ?        Sl   11月28   0:00 /usr/libexec/gsd-rfkill
gdm        2176  0.0  0.3 374360  3068 ?        Sl   11月28   0:00 /usr/libexec/gsd-screensaver-proxy
gdm        2181  0.0  0.4 411848  4376 ?        Sl   11月28   0:00 /usr/libexec/gsd-sharing
gdm        2186  0.0  0.5 472804  5260 ?        Sl   11月28   0:00 /usr/libexec/gsd-smartcard
gdm        2189  0.0  0.4 455260  4940 ?        Sl   11月28   0:00 /usr/libexec/gsd-sound
gdm        2193  0.0  1.6 623604 16628 ?        Sl   11月28   0:00 /usr/libexec/gsd-wacom
colord     2214  0.0  0.6 419772  6396 ?        Ssl  11月28   0:00 /usr/libexec/colord
root       2227  0.0  0.6 163888  6144 ?        Ss   11月28   0:00 sshd: root@pts/0
gdm        2235  0.0  0.3 302356  3416 ?        Sl   11月28   0:00 /usr/libexec/ibus-engine-simple
root       2247  0.0  0.3 117084  3708 pts/0    Ss   11月28   0:00 -bash
root       9764  0.0  0.0      0     0 ?        S    11月28   0:00 [kworker/u256:1]
postfix   11487  0.0  0.4  91976  4116 ?        S    00:00   0:00 pickup -l -t unix -u
root      12241  0.0  0.0      0     0 ?        S    01:16   0:00 [kworker/0:3]
root      12294  0.0  0.0      0     0 ?        S    01:21   0:00 [kworker/0:0]
root      12401  0.0  0.0      0     0 ?        R    01:31   0:00 [kworker/0:1]
root      12444  0.0  0.0 108052   360 ?        S    01:35   0:00 sleep 60
root      12445  0.0  0.1 155448  1876 pts/0    R+   01:35   0:00 ps aux
[root@wxgdfwq-01 soft]# 
