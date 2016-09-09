# apue.2e
APUE source code , Second Edition.

### How to make
1. change Make.defines.linux
vim Make.defines.linux
define your work home
WKDIR=/home/user/apue.2e

2. compile lib apue.a
cd lib
make -f linux.mk

3. compile ipc/popen1.c
gcc popen1.c -o popen1 -I ../include/ -L ../lib -lapue


### Install bins, just like golang
1. create a bin dir at apue.2e, as bin dir, for install bin files
add a line to ~/.bash_profile
apue_bin=/home/larry/apue.2e/bin
source .bash_profile

2. install  
create a install.sh shell script to install your bins to 
or mv bin file to bin dir.

