## **level5.md**

`cd inhere` to go into inhere directory, we can see there are several directories with lots of files, thus file command is not a good option.

instead, use `find`.

`find . -type f -size 1033c ! -executable`, where . stands for current directory, type f is file type, size is for file size and executable flag is to check if it is executable or not.

we will get the required file, `cat` and get the psswd, save it and exit.

