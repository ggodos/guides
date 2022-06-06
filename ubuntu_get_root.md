### How to change ubuntu super user password

1. Enter grub menu (holding shift)
2. Press 'e' on ubuntu, you'll see start script. 
3. Find 'linux    /boot...' line
4. Add in the end of this line " init=/bin/bash"
5. Press Ctrl+X
6. Wait ubuntu su for run and write "mount -o remount,rw /"
7. Write "passwd" and enter new password
8. Write "reboot -f"
9. Profit
