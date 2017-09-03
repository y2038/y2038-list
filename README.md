# y2038-list
A list of what is safe, and not safe from the y2038 Problem. 

## Useful Resources
[KernelNewbies 2038](https://kernelnewbies.org/y2038)


## Kernels
### Linux
### Others

## Syscalls
### Linux
### Windows
### MacOS
### Other

## File Systems
| Filesystem | Time Type | Rollover Date
| --- | --- | --- |
| 9p (9P2000.L) | signed 64-bit seconds, ns | never |
| befs | unsigned 48-bit seconds | never |
| btrfs | signed 64-bit seconds, 32-bit ns | never |
| f2fs | 64-bit seconds / 32-bit ns | never |
| fuse | 64-bit second/32-bit ns | never | 
| gfs2 | u64 seconds/u32 ns | never |
| nfsv4 | u64 seconds/u32 ns | never | 
| nilfs2 | u64 seconds/u32 ns | never |
| omfs | 64-bit milliseconds | never |
| ubifs | u64 second/u32 ns | never |
| ufs2 | signed 64-bit seconds/u32 ns | never | 
| aafs | u32 days/mins/(secs/50) | 11760870 |
| cifs (modern) | 64-bit 100ns since 1601 | 30328 |
| ntfs | 64-bit 100ns since 1601 | 30828 | 
| ext4 (new inodes) | 34 bit seconds / 30-bit ns | 2582 |
| ocfs2 | 34-bit seconds/30-bit ns | 2514| 
| logfs | signed 64-bit ns | 2262 | 
| adfs | 40-bit cs since 1900 | 2248 |
| cifs (smb) | 7-bit years since 1980 | 2107 |
| fat | 7-bit years since 1980, 2s resolution | 2107 |
| ncpfs | 7-bit year since 1980 | 2107 | 
| 9p (9P2000) | unsigned 32-bit seconds | 2106 |
| afs | unsigned 32-bit seconds | 2106 |
| bfs | unsigned 32-bit seconds | 2106 | 
| ceph | unsigned 32-bit second/ns | 2106 |
| efs | unsigned 32-bit seconds | 2106 |
| jffs2 | unsigned 32-bit seconds | 2106 | 
| jfs | unsigned 32-bit seconds/ns | 2106 | 
| freevxfs | unsigned 32-bit seconds/u32 microseconds | 2106 | 
| hpfs | unsigned 32-bit seconds | 2106 |
| minix | unsigned 32-bit seconds | 2106 | 
| nfsv2 | unsigned 32-bit seconds/ns | 2106 | 
| nfsv3 | unsigned 32-bit seconds/ns | 2106 | 
| nfsd | unsigned 32-bit seconds/ns | 2106 | 
| pstore | ascii seconds | 2106 | 
| qnx4 | unsigned 32-bit seconds | 2106 | 
| qnx6 | unsigned 32-bit seconds | 2106 |
| reiserfs | unsigned 32-bit seconds | 2106 |
| romfs | fixed | 1970 | 
| squashfs | unsigned 32-bit seconds | 2106 | 
| sysv | unsigned 32-bit seconds | 2106 | 
| ufs1 | unsigned 32-bit seconds | 2106 | 
| xfs | signed 32-bit seconds/ns | 2106 |
| hfs | u32 seconds since 1904 | 2040 | 
| hfsplus | u32 seconds since 1904 | 2040 | 
| coda | timespec ioctl | 2038 |
| exofs | signed 32-bit seconds | 2038 |
| ext2 | signed 32-bit seconds | 2038 | 
| ext3 | signed 32-bit seconds | 2038
| ext4 (good old inodes) | signed 32-bit seconds | 2038 | 
| hostfs | timespec | 2038 | 
| udf | u16 year | 2038|
| isofs | 'char' year since 1900 (fixable) | 2028 | 
| cramfs | fixed | 1970 | 

Credit to: https://kernelnewbies.org/y2038/vfs for the original list. I have not independently verified it. 

## Core Libraries
### Unix
### Others

## Databases 
* MySQL
* Postgres
* MSSSQL
* SQLLite 
