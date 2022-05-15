### How to change ubuntu super user password

1. Enter grub menu (holding shift)
2. Find '        linux    /boot...'
3. Add in the and of finded line "init=/bin/bash"
4. Press Ctrl+X
5. Wait ubuntu for run and write "mount -o remount,rw /"
6. Write "passwd" and enter new password
7. Write "reboot -f"
8. Profit
