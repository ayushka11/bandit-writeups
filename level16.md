## **level16**

`nmap` is used to scan open ports.

using `nmap -p31000-32000 localhost -sV`, we get the following output:

`Starting Nmap 7.80 ( https://nmap.org ) at 2024-03-18 13:10 UTC`

`Nmap scan report for localhost (127.0.0.1)`

`Host is up (0.00010s latency).`

`Not shown: 996 closed ports`

`PORT      STATE SERVICE     VERSION`

`31046/tcp open  echo`

`31518/tcp open  ssl/echo`

`31691/tcp open  echo`

`31790/tcp open  ssl/unknown`

`31960/tcp open  echo`

we see 2 ports open for ssl, we try both but we get our output from 31790.

same as in prev, we do `openssl s_client -connect 127.0.0.1:31790` and get the RSA key.


