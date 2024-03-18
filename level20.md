## **level20**

we use `nc` command to set up a listening server in the background.

`echo "[current password]" | nc -l -p 6969 & disown`

now, running the binary using `./suconnect 6969` and supplying psswd to it.

`Read : ["current password"]`

`Password matches, sending next password`

save the psswd and exit.

