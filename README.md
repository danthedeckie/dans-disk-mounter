# Dan's Disk Mounter

When you plug in a USB disk, pop up a dialog asking if you want to mount it.
If you say yes, mount it (using pmount).
Then ask if you want to open it with xdg-open (nautilus?)

I use this on my i3 based user, where I don't usually have a file manager etc. running.

Uses the inotify_simple code by Chris Billington, embedded directly into the script so that
there are no dependencies.  You can just copy this to /usr/local/bin/, set it to run on log in,
and away you go.

## Requirements:

- python3
- pmount

## Also included:

a very quick umount_media script, which pops up a dmenu showing mounted /media/ disks, which you can then
select to demount a mounted disk.
