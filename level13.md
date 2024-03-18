## **level13**

`cat sshkey.private` to see the ssh key.

copy the key and change the permissions using below cmd.

`chmod 600 sshkey.private`

now, login to bandit14 using the key

`ssh -i key bandit14@bandit.labs.overthewire.org -p 2220`
