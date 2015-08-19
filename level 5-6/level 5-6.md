ssh bandit5@bandit.labs.overthewire.org

koReBOKuIDDepwhWk7jZC0RTdopnAYKh <enter>

bandit5@melinda:~$ ls

inhere

bandit5@melinda:~$ cd inhere/

bandit5@melinda:~/inhere$ ls -la

total 88

drwxr-x--- 22 root bandit5 4096 Nov 14  2014 .

drwxr-xr-x  3 root root    4096 Nov 14  2014 ..

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere00

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere01

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere02

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere03

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere04

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere05

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere06

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere07

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere08

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere09

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere10

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere11

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere12

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere13

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere14

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere15

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere16

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere17

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere18

drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere19

bandit5@melinda:~/inhere$ find ./ -size 1033c

./maybehere07/.file2

bandit5@melinda:~/inhere$ cat ./maybehere07/.file2

DXjZPULLxYr17uwoI01bNLQbtFemEgo7

bandit5@melinda:~/inhere$ exit

logout

