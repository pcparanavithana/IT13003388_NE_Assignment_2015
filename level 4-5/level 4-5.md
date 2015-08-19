ssh bandit4@bandit.labs.overthewire.org

pIwrPrtPN36QITSp3EQaw936yaFoFgAB <enter>

bandit4@melinda:~$ ls

inhere

bandit4@melinda:~$ cd inhere/

bandit4@melinda:~/inhere$ ls -la

total 48

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file00

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file01

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file02

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file03

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file04

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file05

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file06

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file07

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file08

-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file09

drwxr-xr-x 2 root    root    4096 Nov 14  2014 .

drwxr-xr-x 3 root    root    4096 Nov 14  2014 ..

bandit4@melinda:~/inhere$ file ./-*

./-file00: data

./-file01: data

./-file02: data

./-file03: data

./-file04: data

./-file05: data

./-file06: data

./-file07: ASCII text

./-file08: data

./-file09: data

bandit4@melinda:~/inhere$ cat ./-file07

koReBOKuIDDepwhWk7jZC0RTdopnAYKh

bandit4@melinda:~/inhere$ exit

logout