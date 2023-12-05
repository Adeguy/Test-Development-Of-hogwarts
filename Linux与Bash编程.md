Linux与Bash编程
[ck281183@shell.ceshiren.com ~]$ top
top - 02:14:42 up 4 days, 15:55,  4 users,  load average: 0.10, 0.17, 0.19
Tasks: 107 total,   2 running, 105 sleeping,   0 stopped,   0 zombie
%Cpu(s):  4.0 us,  3.7 sy,  0.0 ni, 92.3 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
KiB Mem :  3879904 total,   111124 free,   540444 used,  3228336 buff/cache
KiB Swap:        0 total,        0 free,        0 used.  2868504 avail Mem 

  PID USER      PR  NI    VIRT    RES    SHR S  %CPU %MEM     TIME+ COMMAND                                                     
 1190 root      10 -10  154144  33248   7264 R   6.6  0.9  80:19.58 AliYunDunMonito                                             
  432 root      20   0  834300  22568   5992 S   0.3  0.6  18:17.34 CmsGoAgent.linu                                             
 9003 root      20   0       0      0      0 S   0.3  0.0   0:00.15 kworker/1:2                                                 
10346 root      20   0  155544   5948   4600 S   0.3  0.2   0:08.89 sshd                                                        
10348 pyqz702+  20   0  156040   3040   1140 S   0.3  0.1   1:05.29 sshd                                                        
    1 root      20   0   43544   3804   2460 S   0.0  0.1   1:30.63 systemd                                                     
    2 root      20   0       0      0      0 S   0.0  0.0   0:00.10 kthreadd                                                    
    4 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 kworker/0:0H                                                
    6 root      20   0       0      0      0 S   0.0  0.0   0:03.74 ksoftirqd/0                                                 
    7 root      rt   0       0      0      0 S   0.0  0.0   0:02.44 migration/0                                                 
    8 root      20   0       0      0      0 S   0.0  0.0   0:00.00 rcu_bh                                                      
    9 root      20   0       0      0      0 S   0.0  0.0   1:23.70 rcu_sched                                                   
   10 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 lru-add-drain                                               
   13 root      rt   0       0      0      0 S   0.0  0.0   0:03.05 migration/1                                                 
   14 root      20   0       0      0      0 S   0.0  0.0   0:03.72 ksoftirqd/1                                                 
   16 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 kworker/1:0H                                                
   18 root      20   0       0      0      0 S   0.0  0.0   0:00.00 kdevtmpfs                                                   
   19 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 netns                                                       
   20 root      20   0       0      0      0 S   0.0  0.0   0:00.12 khungtaskd                                                  
   21 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 writeback                                                   
   22 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 kintegrityd                                                 
   23 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 bioset                                                      
   24 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 bioset                                                      
   25 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 bioset                                                      
   26 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 kblockd                                                     
   27 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 md                                                          
   28 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 edac-poller                                                 
   29 root       0 -20       0      0      0 S   0.0  0.0   0:00.00 watchdogd                                                   
   36 root      20   0       0      0      0 S   0.0  0.0   0:02.30 kswapd0            
[ck281183@shell.ceshiren.com home]$ ls |wc -w
8586
[ck281183@shell.ceshiren.com home]$ netstat -anp|awk 'NR>2{print $6}'|grep -i -E 'connect|listen'|uniq -c
(No info could be read for "-p": geteuid()=10474 but you should be root.)
      7 LISTEN
     58 CONNECTED

