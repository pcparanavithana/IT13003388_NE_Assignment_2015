ssh bandit12@bandit.labs.overthewire.org

5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu <enter>

bandit12@melinda:~$ ls

data.txt
bandit12@melinda:~$ file data.txt 

data.txt: ASCII text
bandit12@melinda:~$ mkdir /temp/stw

mkdir: cannot create directory '/temp/stw': No such file or directory
bandit12@melinda:~$ cd /tmp/stw

bandit12@melinda:/tmp/stw$ xxd -r ~/data.txt > data.txt

bandit12@melinda:/tmp/stw$ file data.txt

data.txt: gzip compressed data, was "data2.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/stw$


bandit12@melinda:/tmp/stw$ zcat data.txt > dataNew

bandit12@melinda:/tmp/stw$ ls

data.txt  data5.bin  data6.bin  data6.bin.out  data8.bin  dataNew  dataNew.out  evenNewer  lost  newer  nnewer
bandit12@melinda:/tmp/stw$ file dataNew
dataNew: bzip2 compressed data, block size = 900k
bandit12@melinda:/tmp/stw$ bzip2 -d dataNew
bzip2: Can't guess original name for dataNew -- using dataNew.out
bzip2: Output file dataNew.out already exists.

bandit12@melinda:/tmp/stw$ ls

data.txt  data5.bin  data6.bin  data6.bin.out  data8.bin  dataNew  dataNew.out  evenNewer  lost  newer  nnewer

bandit12@melinda:/tmp/stw$ file dataNew.out
dataNew.out: gzip compressed data, was "data4.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression

bandit12@melinda:/tmp/stw$ zcat dataNew.out > evenNewer

bandit12@melinda:/tmp/stw$ ls

data.txt  data5.bin  data6.bin  data6.bin.out  data8.bin  dataNew  dataNew.out  evenNewer  lost  newer  nnewer

bandit12@melinda:/tmp/stw$ file evenNewer

evenNewer: POSIX tar archive (GNU)

bandit12@melinda:/tmp/stw$ tar -xvf evenNewer
data5.bin

bandit12@melinda:/tmp/stw$ file data5.bin

data5.bin: POSIX tar archive (GNU)


bandit12@melinda:/tmp/stw$ tar -xvf data5.bin
data6.bin

bandit12@melinda:/tmp/stw$ file data6.bin

data6.bin: bzip2 compressed data, block size = 900k

bandit12@melinda:/tmp/stw$ bzip2 -d data6.bin

bzip2: Can't guess original name for data6.bin -- using data6.bin.out

bzip2: Output file data6.bin.out already exists.

bandit12@melinda:/tmp/stw$ ls

data.txt  data5.bin  data6.bin  data6.bin.out  data8.bin  dataNew  dataNew.out  evenNewer  lost  newer  nnewer

bandit12@melinda:/tmp/stw$ file data6.bin.out

data6.bin.out: POSIX tar archive (GNU)

bandit12@melinda:/tmp/stw$ tar -xvf data6.bin.out
data8.bin

bandit12@melinda:/tmp/stw$ file data8.bin

data8.bin: gzip compressed data, was "data9.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression


bandit12@melinda:/tmp/stw$ zcat data8.bin > lost

bandit12@melinda:/tmp/stw$ ls

data.txt  data5.bin  data6.bin  data6.bin.out  data8.bin  dataNew  dataNew.out  evenNewer  lost  newer  nnewer

bandit12@melinda:/tmp/stw$ file lost

lost: ASCII text

bandit12@melinda:/tmp/stw$ cat lost

The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

bandit12@melinda:/tmp/stw$ exit

logout
