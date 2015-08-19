bandit21@melissa:~$ cd /etc/cron.d/

bandit21@melissa:/etc/cron.d$ ls -la

total 100

drwxr-xr-x  2 root root 4096 2013-01-03 16:39 .

drwxr-xr-x 94 root root 4096 2013-03-18 15:53 ..

-rw-r--r--  1 root root   54 2013-01-03 16:39 boobiesbot-check

-rw-r--r--  1 root root   61 2012-07-05 09:34 
cronjob_bandit22

-rw-r--r--  1 root root   61 2012-07-05 09:34 cronjob_bandit23

-rw-r--r--  1 root root   61 2012-07-05 09:35 cronjob_bandit24

-rw-r--r--  1 root root   35 2012-03-29 14:16 eloi0

-rw-r--r--  1 root root   35 2012-04-07 18:33 eloi1

-rw-r--r--  1 root root   51 2012-12-23 00:06 hintbot-check

-rw-------  1 root root  233 2012-09-14 13:16 
manpage3_resetpw_job

-rw-r--r--  1 root root  506 2012-06-19 03:06 php5

-rw-r--r--  1 root root  102 2011-01-05 11:23 .placeholder

-rw-r--r--  1 root root   58 2011-11-13 23:08 semtex0-32

-rw-r--r--  1 root root   58 2011-11-13 23:08 semtex0-64

-rw-r--r--  1 root root   59 2011-11-13 23:08 semtex0-ppc

-rw-r--r--  1 root root   36 2011-11-25 14:00 semtex10

-rw-r--r--  1 root root  143 2011-11-13 23:08 semtex12

-rw-r--r--  1 root root   35 2011-11-13 23:08 semtex5

-rw-r--r--  1 root root   29 2011-11-13 23:08 semtex6

-rw-r--r--  1 root root   96 2011-11-25 14:00 semtex8

-rw-r--r--  1 root root  134 2011-11-13 23:14 semtex9

-rw-r--r--  1 root root   29 2011-11-13 23:07 vortex0

-rw-r--r--  1 root root   30 2012-03-24 21:00 vortex20

-rw-r--r--  1 root root   52 2012-12-23 00:06 vulnbot0-check

-rw-r--r--  1 root root   52 2012-12-23 00:06 vulnbot1-check

bandit21@melissa:/etc/cron.d$ cat cronjob_bandit22
bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null

bandit21@melissa:/etc/cron.d$ cat /usr/bin/cronjob_bandit22.sh

//#!/bin/bash

chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
bandit21@melissa:/etc/cron.d$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI