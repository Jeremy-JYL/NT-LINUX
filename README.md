# NT-LINUX
A simple ARM Linux initrd with busybox and glibc

# Edit initrd

To edit initrd first, download v** - **** initrd download both file initrd.gz and mkinit.
Next, first check cpio is working with `cpio` else you need to install one.
After this, you can unzip the .gz file with `tar -xvf initrd.gz`
Then, create a folder called root and `cd root` finally `gzip -cd ../initrd.gz | cpio -idmv`
Finally, the initrd files are in root folder
After you finish editing, `cd ..`, then `sh ./mkinit` or `./mkinit` and you finished editing the NT LINUX initrd files.
