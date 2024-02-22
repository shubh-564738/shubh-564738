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
***Check File/Folder/Content (LS, LL, CAT, GREP, HEAD, TAIL, LESS, MORE, ECHO)**
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

root@shubham-Latitude-7480:~# 


