# Backup for Libvirt/KVM VMs
vm-backup can be used to make offline or online backups of libvirt/KVM virtual machines.

## Usage

```
$ /opt/bin/vm-backup 
Usage: ./vm-backup <backup-folder> <domain> <host>
```
```
Options:
    <backup-folder> Copy images to the specified <directory>
    <domain>        Name of the instace to backup
    <host>          Can be localhost|127.0.0.1 or FQDN
```

```
Example:
$ /opt/bin/vm-backup /backup myvm myhost
Beginning backup for myvm

Starting backup of VM myvm to /backup/myvm/2019.04.10.143259
Creating backup subdirectories /backup/myvm/2019.04.10.143259
sending incremental file list
disk.0
          1.17G 100%   92.90MB/s    0:00:11 (xfr#1, to-chk=0/1)
Finished backup
```

## License

2-clause license ("Simplified BSD License" or "FreeBSD License")
