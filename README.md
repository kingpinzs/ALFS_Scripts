Where I am going to store my linux from scratch scripts

run bash version-check.sh from the LFS book in case things change
version LFS 11.2 
sudo ln -sf bash /bin/sh
apt install binutils-dev bison gawk make gcc-10 build-essential texinfo

export LFS=/mnt/lfs

add your user to the sudoers
usermod -aG sudo [username] <----Your username goes here
or run
EDITOR=nano visudo
add this line 
[username]  ALL=(ALL) NOPASSWD:ALL


ALFS
bash required_software.sh

git clone https://git.linuxfromscratch.org/jhalfs.git
