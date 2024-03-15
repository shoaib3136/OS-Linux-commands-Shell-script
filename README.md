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
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/924b5e4f-b6d9-4ce3-894b-2b1edbf587c0)



cat > file22

1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
 
uniq file22
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/94e1fa19-3646-4f72-97c8-eff4a0e11279)




#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
 ![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/b286bcd8-f51d-4f2b-a6ae-c06dd89621f6)


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
 ![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/de7ce8af-1855-4dec-99f3-734859a20a00)



 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/255942df-5e83-4d32-b128-ee2fe540cebe)




#Backup commands
tar -cvf backup.tar *
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/8c62851c-a964-43f2-86cc-74216fecdaf3)

 
cat << stop > herecheck.txt

hello in this world

i cant stop

for this non stop movement

stop



cat herecheck.txt
## OUTPUT
![image](https://github.com/shoaib3136/OS-Linux-commands-Shell-script/assets/117919362/3eb2f341-b2a9-463b-9314-97f5a3971a76)


# RESULT:
The Commands are executed successfully.
