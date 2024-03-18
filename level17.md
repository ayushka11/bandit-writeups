## **level17**

we first save the ssh key in a file.

then login using, `ssh -i {sshkey file} bandit17@bandit.labs.overthewire.org -p 2220`

we need to find the unique line in passwords.new which is not there in passwords.old.

we do this using `diff` command to find difference between two files.

`diff passwords.new passwords.old` will give two lines unique to passwords.new and passwords.old respectively.

So, the first string is our psswd, save it and exit.



