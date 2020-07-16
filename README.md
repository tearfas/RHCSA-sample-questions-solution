# RHCSA-sample-questions-solution  
RHCSA sample questions/solution -- http://www.certificationking.com/download/RHCSA.htm


Question: 1   
<<<<<<< HEAD

=======
>>>>>>> master
Configure your Host Name, IP Address, Gateway and DNS.
Host name: rhcsa.dellatechglobal.com                  
IP Address: 192.168.0.57/24                 
Gateway: 192.168.0.1                                 
DNS:192.168.0.1                                  
DNS Search: dellatechglobal.com  
  
 
 
Question: 2   
<<<<<<< HEAD

=======
>>>>>>> master
Add 3 users: harry, natasha, tom.
The requirements: The Additional group of the two users: harry, Natasha is the admin
group. The user: tom's login shell should be non‐interactive.  
  
 
Question: 3      

Create a catalog under /home named admins. Its respective group is requested to be
the admin group. The group users could read and write, while
other users are not allowed to access it. The files created by users from the same group
should also be the admin group.  

 
Question: 4   

Configure a task: plan to run echo hello command at 14:23 every day.  
 
 
Question: 5   

Find the files owned by harry, and copy it to catalog: /opt/dir 
 
 
Question: 6      

Find the rows that contain abcde from file /etc/testfile, and write it to the
file/tmp/testfile, and the sequence is requested as the same as /etc/testfile.
 
 
Question: 7   

Create a 2G swap partition which take effect automatically at boot‐start, and it should
not affect the original swap partition.  
 
Question: 8   

Create a user named alex, and the user id should be 1234, and the password should be
alex111.  
 
 
Question: 9      

Install a FTP server, and request to anonymous download from /var/ftp/pub catalog. (it
needs you to configure yum direct to the already existing file
server.) 
 
 
Question: 10   

Configure a HTTP server, which can be accessed through
http://station.domain40.example.com.
Please download the released page from http://ip/dir/example.html.  
 
Question: 11   

Configure the verification mode of your host account and the password as LDAP. And it
can login successfully through ldapuser40. The password is set
as "password". And the certificate can be downloaded from http://ip/dir/ldap.crt. After
the user logs on the user has no host directory unless you
configure the autofs in the following questions. 
 
 
Question: 12      

Configure autofs to make sure after login successfully, it has the home directory autofs,
which is shared as /rhome/ldapuser40 at the ip: 172.24.40.10.
and it also requires that, other ldap users can use the home directory normally.  

 
 
Question: 13   

Configure the system synchronous as 172.24.40.10.  
 
 
Question: 14   

Change the logical volume capacity named vo from 190M to 300M. and the size of the
floating range should set between 280 and 320. (This logical
volume has been mounted in advance.)  
  

Question: 15      

Create a volume group, and set 16M as a extends. And divided a volume group
containing 50 extends on volume group lv, make it as ext4 file system,
and mounted automatically under /mnt/data.  
 
Question: 16   

Upgrading the kernel as 2.6.36.7.1, and configure the system to Start the default kernel,
keep the old kernel available.  
 
 
Question: 17   

Create a 512M partition, make it as ext4 file system, mounted automatically under
/mnt/data and which take effect automatically at boot‐start.  
 
 
Question: 18      

Create a volume group, and set 8M as a extends. Divided a volume group containing 50
extends on volume group lv (lvshare), make it as ext4 file
system, and mounted automatically under /mnt/data. And the size of the floating range
should set between 380M and 400M. 
 
 
Question: 19   

Download ftp://192.168.0.254/pub/boot.iso to /root, and mounted automatically under
/media/cdrom and which take effect automatically at boot‐start.  
 
 
Question: 20   

Add admin group and set gid=600  
 
 
Question: 21      

Add user: user1, set uid=601
Password: redhat
The user's login shell should be non‐interactive.  
Answer: See explanation below.
 
Question: 22   

Add users: user2, user3.
The Additional group of the two users: user2, user3 is the admin group Password:
redhat  
 
 
Question: 23   

Copy /etc/fstab to /var/tmp name admin, the user1 could read, write and modify it,
while user2 without any permission.  
 
 
Question: 24      

Configure a task: plan to run echo "file" command at 14:23 every day.  

 
Question: 25   

Configure a default software repository for your system.
One YUM has already provided to configure your system on
http://server.domain11.example.com/pub/ x86_64/Server, and can be used normally.  
 
Question: 26   

Adjust the size of the Logical Volume.
Adjust the size of the vo Logical Volume, its file system size should be 290M. Make sure
that the content of this system is complete.
Note: the partition size is rarely accurate to the same size as required, so in the range
270M to 320M is acceptable.
 
Question: 27      

Create User Account.
Create the following user, group and group membership:
Adminuser group
User natasha, using adminuser as a sub group
User Harry, also using adminuser as a sub group
User sarah, can not access the SHELL which is interactive in the system, and is not a
member of adminuser, natasha harry sarah password is redhat.  

 
 
Question: 28   

Configure /var/tmp/fstab Permission.
Copy the file /etc/fstab to /var/tmp/fstab. Configure var/tmp/fstab permissions as the
following:
Owner of the file /var/tmp/fstab is Root, belongs to group root
File /var/tmp/fstab cannot be executed by any user
User natasha can read and write /var/tmp/fstab
User harry cannot read and write /var/tmp/fstab
All other users (present and future) can read var/tmp/fstab.  
 
Question: 29   

Configure a cron Task.
User natasha must configure a cron job, local time 14:23 runs and executes: */bin/echo
hiya every day. 
 
Question: 30      

Create a Shared Directory.
Create a shared directory /home/admins, make it has the following characteristics:
/home/admins belongs to group adminuser
This directory can be read and written by members of group adminuser Any files
created in /home/ admin, group automatically set as adminuser.  

 
Question: 31   

Install the Kernel Upgrade.
Install suitable kernel update from:
http://server.domain11.example.com/pub/updates.
Following requirements must be met:
Updated kernel used as the default kernel of system start‐up.
The original kernel is still valid and can be guided when system starts up.  
 
 
Question: 32   

Binding to an external validation server.
System server.domain11.example.com provides a LDAP validation service, your system
should bind to this service as required:
Base DN of validation service is dc=example,dc=com
LDAP is used for providing account information and validation information Connecting
and using the certification of http://server.domain11.example.com/
pub/EXAMPLE‐CA‐CERT to encrypt
After the correct configuration, ldapuser1 can log into your system, it does not have
HOME directory until you finish autofs questions, ldapuser1
password is password.  
 
 
Question: 33      

Configure NTP.
Configure NTP service, Synchronize the server time, NTP server: classroom.example.com  

 
Question: 34   

Configure autofs.
Configure the autofs automatically mount to the home directory of LDAP, as required:
server.domain11.example.com use NFS to share the home to your system. This file
system contains a pre
configured home directory of user ldapuserX.
Home directory of ldapuserX is:
server.domain11.example.com /home/guests/ldapuser
Home directory of ldapuserX should automatically mount to the ldapuserX of the local
/home/guests Home directory’s write permissions must be
available for users ldapuser1’s password is password  
