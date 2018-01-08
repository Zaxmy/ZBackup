# ZBackup :shell:

Make daily backups of ZFS filesystems to a remote ZFS server over SSH.

Makes daily snapshots and sends data incrementally from last common snapshot. 

## Usage :speech_balloon:
```
usage: ZBackup [-h] -f FILESYSTEM -b BACKUPHOST [-u BACKUPUSER] [-s SSH]
               [-z ZFS] [-p ZPOOL] [-d] [--version]

optional arguments:
  -h, --help            show this help message and exit

Server side options:
  -f FILESYSTEM, --filesystem FILESYSTEM
                        Filesystem to backup, multiple possible

Backup server options:
  -b BACKUPHOST, --backup-server BACKUPHOST
                        Server to send backups to
  -u BACKUPUSER, --user BACKUPUSER
                        Remote user

Other:
  -s SSH, --ssh SSH     Absolute path to SSH binary
  -z ZFS, --zfs ZFS     Absolute path to zfs binary
  -p ZPOOL, --zpool ZPOOL
                        Absolute path to zpool binary
  -d, --debug           Turns on debugging
  --version             show program's version number and exit
```
