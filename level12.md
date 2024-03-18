## **level12**

we first copy the data file to /tmp using below `mkdir`, `cd`, `cp` commands.

`mkdir /tmp/ayu`
`cd /tmp/ayu`
`cp ~/data.txt .`

using `xxd -r data.txt data` to reverse the hexdump.

we use `file data` to see that this file is a gzip compressed file.

we need to rename and decompress it.

`mv data data.gz && gzip -d data.gz`, mv to rename and gzip -d to decompress.

we use `file data` to see that it is a bzip2 archive.

using `bzip2 -d data` to decompress this.

`file data.out` to see that it is again a gz archive.

`mv data.out data.gz && gzip -d data.gz`, same command as above but with different file name.

`ls` to see that it contains a file data

`file data` 
output - `data: POSIX tar archive (GNU)`

these files have extension .tar and can be decompressed using `tar -xvf filename`, repeating these steps until we reach a file with ascii text.

cat the output, save the psswd and exit.



