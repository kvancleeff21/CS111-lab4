# Hey! I'm Filing Here

In this lab, I successfully implemented the ext2 filesystem, and more specifically, I implemented functions
that allow this program to mount and partition a 1 MiB array of bytes. The functions I implemented deal with creating 
the superblock, the block group descriptor table, block bitmap, inode bitmap, inode table, the root directory, and then function that
creates the specific files I'm tasked with creating such as the hello-world regular file and a hello symlink file. 

## Building

make
./ext2-create

## Running

fsck.ext2 cs111-base.img
dumpe2fs cs111-base.img
mkdir mnt
sudo mount -o loop cs111-base.img mnt


## Cleaning up

sudo umount mnt
rmdir mnt
make clean
