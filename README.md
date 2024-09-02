## Name
Snaputils
## Description
simple Zfs snap frontends to use snapshots -"snap" and "snapnkeep"
most useful for non-root/sudo user in their home directory
try "snap -h" for help
I use "snapnkeep" in daily.local to keep a week or so worth d0-d7 of snapshot. you can use that template in crontab to keep hourly snapshots.  
## Usage
"snap ls"
"snap ls d3
"snap ls -l d3:foo.c"
"snap diff d0:foo.c"
"snap get d2:foo.c" - replaces current file  
"snap list".
"snap create" or snap destroy works with sudo. but I generally use the normal zfs command for that.
Use the "-n" (dryrun) option to check it will do what you expect first!
#
