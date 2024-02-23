**Q File and Folder Create Command (TOUCH, MKDIR, VIM )**
```
touch filea
mkdir dir1
vim filea
cat filea  (hello 
this is shubham)
ls  -  dir1  filea  shubham
```
**Q File and Folder Permission CHOWN, CHMOD, CHGRP)**
```
sudo chown boxer filea
ls -l
-rw-r--r--  1 boxer   root      25 Feb 21 11:42 filea
drwxr-x--- 21 shubham shubham 4096 Feb 21 11:27 shubham

ls -l
-rw-r--r--  1 shubham root      32 Feb 21 13:28 filea
drwxr-x--- 21 shubham shubham 4096 Feb 21 11:27 shubham
chmod 777 filea
ls -l
-rwxrwxrwx  1 shubham root      32 Feb 21 13:28 filea
drwxr-x--- 21 shubham shubham 4096 Feb 21 11:27 shubham

chgrp boxer filea
 ls -l
-rwxrwxrwx  1 shubham boxer     32 Feb 21 13:28 filea
drwxr-x--- 21 shubham shubham 4096 Feb 21 11:27 shubham
```
**Q Check File/Folder/Content (LS, LL, CAT, GREP, HEAD, TAIL, LESS, MORE, ECHO)**
```
ls
filea  shubham

ll
drwxr-xr-x  3 root    root    4096 Feb 21 13:28 ./
drwxr-xr-x 20 root    root    4096 Jan  7 22:55 ../
-rwxrwxrwx  1 shubham boxer     32 Feb 21 13:28 filea*
drwxr-x--- 21 shubham shubham 4096 Feb 21 11:27 shubham/

cat filea
hello 
this is shubham

touch a.txt b.txt c.txt d.txt 
ls
a.txt  b.txt  c.txt  d.txt  filea  shubham
ls > file_list.txt
cat file_list.txt
a.txt
b.txt
c.txt
d.txt
filea
file_list.txt
shubham
cat file_list.txt |grep .txt
a.txt
b.txt
c.txt
d.txt
file_list.txt

root@shubham-Latitude-7480:~# cat a.txt
a
b
c
d
e
f
g
h
i
j
k
l
m
n
o
p
root@shubham-Latitude-7480:~# head a.txt
a
b
c
d
e
f
g
h
i
j
root@shubham-Latitude-7480:~# 

root@shubham-Latitude-7480:~# tail a.txt
h
i
j
k
l
m
n
o
p

root@shubham-Latitude-7480:/home# less a.txt

a
b
c
d
e
f
g
h
i
j
k
l
m
n
o
p
q
r
s
t
u
v


root@shubham-Latitude-7480:/home# more a.txt

a
b
c
d
e
f
g
h
i
j
k
l
m
n
o
p
q
r
s
t
u
v
w
x
y
z
aa
ab
ac
ad
ae
af
ag
ah
ai


root@shubham-Latitude-7480:/home# current_date=$(date)
root@shubham-Latitude-7480:/home# echo $current_date
Friday 23 February 2024 10:16:04 PM IST
root@shubham-Latitude-7480:/home# echo $current_date >>b.txt
root@shubham-Latitude-7480:/home# cat b.txt
hello world

Friday 23 February 2024 10:16:04 PM IST
root@shubham-Latitude-7480:/home# echo "I am adding a new line" >>b.txt
root@shubham-Latitude-7480:/home# cat b.txt
hello world

Friday 23 February 2024 10:16:04 PM IST
I am adding a new line


**Q Copy and Move Command (RM, CP, MV, SCP, RSYNC)**

root@shubham-Latitude-7480:/home# ls
a.txt  b.txt  c.txt  d.txt  filea  file_list.txt  shubham
root@shubham-Latitude-7480:/home# rm filea
root@shubham-Latitude-7480:/home# ls
a.txt  b.txt  c.txt  d.txt  file_list.txt  shubham


root@shubham-Latitude-7480:/home# cat b.txt
hello world

Friday 23 February 2024 10:16:04 PM IST
I am adding a new line
root@shubham-Latitude-7480:/home# cp b.txt c.txt
root@shubham-Latitude-7480:/home# cat c.txt
hello world

Friday 23 February 2024 10:16:04 PM IST
I am adding a new line


root@shubham-Latitude-7480:/home# vi filea
root@shubham-Latitude-7480:/home# cat filea
hello all

root@shubham-Latitude-7480:/home# touch fileb
root@shubham-Latitude-7480:/home# mv filea fileb
root@shubham-Latitude-7480:/home# cat fileb
hello all





