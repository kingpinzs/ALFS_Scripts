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

wget https://www.kernel.org/pub/linux/kernel/v5.x/linux-5.19.8.tar.xz
create the .config file to be used later
sudo apt-get install libncurses5-dev libncursesw5-dev flex

make mrproper
make defconfig

git clone https://git.linuxfromscratch.org/jhalfs.git
