# TODO to improve this set of systemd scripts

There is currently a few items hard-coding the base directory of the system to `/opt/MC` in the systemd scripts.

My goal is to change that, allowingany base directory so chosen by the user.


## Early Ideas ##

- Create a script to generate the various systemd unit files
   - The script may be in a variety of languages
      - Python seems to be a good contender
      - Simple shell script is good for the unix and linux crowd
      - PowerShell script seems an interesting contender for Windows systems


## Files with Hard-Coded References ##

Several files contain hard-coded references to directories, files, and usernames.


### References to: /opt/MC ###

The following files contain _hard-coded_ references to `/opt/MC`:

- mcbackup@.service
- mc@.service
- mcbe@.service
- mcbe-backup@.service
- mcbe-autoupdate@.service
- mcbe-getzip@.service


### References to the user 'mc' ###

_Note that I did **not** document these, however, there are plenty of them._

