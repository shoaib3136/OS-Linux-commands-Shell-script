# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1

chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d

cat > file2

anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d

### Display the content of the files
cat < file1
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/0119401d-8e53-42c4-ab54-ce749dc6a03e)





cat < file2
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/9d6b43a7-9146-4ad3-bd12-6124400fb4d7)



# Comparing Files
cmp file1 file2
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/ec7146a1-7dcf-4519-b2bd-bb074874a9f6)

 
comm file1 file2
 ## OUTPUT
 ![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/2b388c18-8716-471f-86a5-104b81593a8b)


 
diff file1 file2
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/bdc3e442-d591-40aa-b92a-121299adbb65)


#Filters

### Create the following files file11, file22 as follows:

cat > file11

Hello world

This is my world

^d

cat > file22

1001 | Ram | 10000 | HR

1002 | tom |  5000 | Admin

1003 | Joe |  7000 | Developer

^d



cut -c1-3 file11
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/141e89e4-c3d8-4296-b12d-a2e6bb80f2df)





cut -d "|" -f 1 file22
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/b1f5d32d-f1a3-4a66-9c0e-10d02548f316)



cut -d "|" -f 2 file22
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/336fe232-b5b0-424a-88fe-5ca75d10039f)

cat < newfile 

Hello world

hello world

^d
`
cat > newfile 

Hello world

hello world

^d
 
grep Hello newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/fc26c416-54b1-4b9c-b839-1e6a77c2ff12)




grep hello newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/3cfe2166-0ee0-46f4-9b7c-44512aeae4cd)





grep -v hello newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/d6dd2db3-b402-47b5-84f7-35e3b2038e37)




cat newfile | grep -i "hello"
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/eb5b87a0-bb58-4854-a95f-1063a74d1320)





cat newfile | grep -i -c "hello"
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/3c2aa26a-270d-42cf-9f04-ce10dc341942)





grep -R ubuntu /etc
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/04c00dca-5051-48a8-9333-c20a7bfd9328)




grep -w -n world newfile   
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/a08e3266-9005-4680-b75a-cb7687d0b869)



cat < newfile 

Hello world

hello world

Linux is world number 1

Unix is predecessor

Linux is best in this World

^d


cat > newfile

Hello world

hello world

Linux is world number 1

Unix is predecessor

Linux is best in this World

^d
 
egrep -w 'Hello|hello' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/2e1abf54-ea02-4eb8-b1f6-fff5fef677e0)





egrep -w '(H|h)ello' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/618c12f7-7069-417f-8616-481edb3859ad)






egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/cc45623c-2d8c-40a7-901e-488b36d5ed02)




egrep '(^hello)' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/b44ed469-befa-4fb3-a15e-41324eaca2dc)




egrep '(world$)' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/705b8878-2407-4f14-b7ec-1a92f9a81314)




egrep '(World$)' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/740a21f7-daab-4ba2-8a61-4c282f7e7766)



egrep '((W|w)orld$)' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/25ac512f-2dfb-4038-925f-0b2818d8a912)




egrep '[1-9]' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/27139ca7-cf2a-4851-8047-cd30f39b3da4)




egrep 'Linux.*world' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/65f9c469-4f04-4490-b7b8-75268e22fbce)



egrep 'Linux.*World' newfile 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/82dd6efa-a158-4a99-b1d3-60ec8d16d18c)



egrep l{2} newfile
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/7878b983-dcc0-4fad-96df-0eabfaff7a9c)




egrep 's{1,2}' newfile
## OUTPUT 
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/5743baa7-5209-46b3-89ff-1398ce18f46d)



cat > file23

1001 | Ram | 10000 | HR

1001 | Ram | 10000 | HR

1002 | tom |  5000 | Admin

1003 | Joe |  7000 | Developer

1005 | Sam |  5000 | HR

1004 | Sit |  7000 | Dev 

1003 | Joe |  7000 | Developer

1001 | Ram | 10000 | HR

^d



sed -n -e '3p' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/6ea57d36-ce6c-4daf-8d42-39476d4518a4)




sed -n -e '$p' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/ecf7119f-656f-4dfe-89fa-6e49e0f9104c)




sed  -e 's/Ram/Sita/' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/677587a1-2033-4bcc-8394-4e7253d8906c)




sed  -e '2s/Ram/Sita/' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/b00debdd-71b6-4595-8af4-8dd502d1e9d1)




sed  '/tom/s/5000/6000/' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/8f6fb32f-68c3-4685-8377-895403873fdf)




sed -n -e '1,5p' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/a57f600b-bf98-4ccf-8ea3-c966a7e7097c)




sed -n -e '2,/Joe/p' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/65246582-bd0f-490b-8352-01ff92960b8f)






sed -n -e '/tom/,/Joe/p' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/ca015e97-51d3-46b3-a4b2-883386487e96)



seq 10 
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/d89684e2-6e84-4c92-b8f7-05a1c425b8f6)




seq 10 | sed -n '4,6p'
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/f2346439-9a61-4e57-a9fb-66a7fe066be9)




seq 10 | sed -n '2,~4p'
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/782ae142-f59f-4252-a128-61f12027a343)




seq 3 | sed '2a hello'
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/a198c8b4-6c65-4fe9-ba15-3b9106f603af)




seq 2 | sed '2i hello'
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/cc2be9dc-529d-48a8-8006-8d9658906ac7)



seq 10 | sed '2,9c hello'
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/1ff68b19-cd1a-4152-930d-191cdf0a400a)



sed -n '2,4{s/^/$/;p}' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/26180a7a-ef81-4172-b7aa-275a1a5545b3)




sed -n '2,4{s/$/*/;p}' file23
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/4082ae2d-91db-4998-95a9-336e7a63e3e4)



#Sorting File content
cat > file21

1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
 
sort file21
## OUTPUT


cat > file22

1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
 
uniq file22
## OUTPUT



#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT

cat < urllist.txt

www. yahoo. com
www. google. com
www. mrcet.... com
^d
 
cat > urllist.txt

www. yahoo. com
www. google. com
www. mrcet.... com
 
cat urllist.txt | tr -d ' '
 ## OUTPUT


 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT



#Backup commands
tar -cvf backup.tar *
## OUTPUT


mkdir backupdir
 
mv backup.tar backupdir
 
tar -tvf backup.tar
## OUTPUT


tar -xvf backup.tar
## OUTPUT

gzip backup.tar

ls .gz
## OUTPUT
 
gunzip backup.tar.gz
## OUTPUT

 
# Shell Script

echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh

chmod 755 my-script.sh
./my-script.sh
## OUTPUT

 
cat << stop > herecheck.txt

hello in this world
i cant stop
for this non stop movement
stop


cat herecheck.txt
## OUTPUT


cat < scriptest.sh 
bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 

cat scriptest.sh 
bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps

 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT

 
ls file1
## OUTPUT

echo $?
## OUTPUT 
./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 
abcd
 
echo $?
 ## OUTPUT


 
# mis-using string comparisons

cat < strcomp.sh 
bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d


cat strcomp.sh 
bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi

##OUTPUT



chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT


# check file ownership
cat < psswdperm.sh 
bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d


cat psswdperm.sh 
bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 
./psswdperm.sh
## OUTPUT

# check if with file location
cat>ifnested.sh 
bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d

cat ifnested.sh 

\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi


./ifnested.sh 
## OUTPUT



# using numeric test comparisons
cat > iftest.sh 
bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d



cat iftest.sh 
bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi


$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT

# check if a file
cat > ifnested.sh 
bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d


cat ifnested.sh 
bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi


$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT

# looking for a possible value using elif
cat elifcheck.sh 
bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi


$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT


# testing compound comparisons
cat> ifcompound.sh 
bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi

$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT

# using the case command
cat >casecheck.sh 
bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac

$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
 
cat > whiletest
bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done

$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 
 
cat untiltest.sh 
bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
 
$ chmod 755 untiltest.sh
 
 
 
cat forin1.sh 
bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 
 
$ chmod 755 forin1.sh
 
 
cat forin2.sh 
bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 
 
$ chmod 755 forin2.sh
 
cat forin2.sh 
bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done

$ chmod 755 forin2.sh
 
$ ./forin2.sh 
 
cat forin3.sh 
bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done

$ ./forin3.sh 
 
cat forin1.sh 
bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done

$ chmod 755 forin1.sh

## OUTPUT
cat forinfile.sh 
bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done

$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT


cat forctype.sh 
bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
`
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT

cat forctype1.sh 
bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done

$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT

cat fornested1.sh 
bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done

$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT

 
cat forbreak.sh 
bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“

## OUTPUT

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“


 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 
cat exread.sh 
bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT


 cat exread1.sh
bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
 
$ chmod 755 exread1.sh 

## OUTPUT



$ ./exread1.sh 
 
cat funcex.sh
bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi

## OUTPUT
 ./funcex.sh 

 
 ./funcex.sh 1 2

 
cat argshift.sh
bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done

$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 
 cat argshift1.sh
bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done

$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 
cat argshift.sh
bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x

## OUTPUT
 ./argshift.sh 1 2 3
 
 
cat > nc.awk
bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 
cat>data.dat
bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj

awk -f nc.awk data.dat
## OUTPUT 
 
cat > palindrome.sh
bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi

## OUTPUT 


# RESULT:
The Commands are executed successfully.
