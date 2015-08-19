ssh bandit20@bandit.labs.overthewire.org

GbKksEFF4yrVs6il55v6gwY5aVje5f0j <enter>


bandit20@melinda:~$ ls

suconnect

bandit20@melinda:~$ ./suconnect

Usage: ./suconnect <portnumber>

This program will connect to the given port on localhost using TCP. If it receives the correct password from the other side, the next password is transmitted back.

#in first shell

bandit20@melinda:~$ nc -l 3222


#in second shell

bandit20@melinda:~$ ls

suconnect

bandit20@melinda:~$ ./suconnect 3222



#When the connection is made, go back to the first shell, and paste the password in netcat.

GbKksEFF4yrVs6il55v6gwY5aVje5f0j

gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
 
Read: GbKksEFF4yrVs6il55v6gwY5aVje5f0j

Password matches, sending next password