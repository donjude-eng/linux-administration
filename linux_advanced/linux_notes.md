# syslog standard
* Aids in the processing of messages
* Allows logging to be centrally controlled.
* Uses facilities and severities to categorize messages.

# Test logrotate configuration
* logrotate -fv /etc/logrotate.conf

# Summary
* The syslog standard
* facilities and severties
* Syslog servers
* logging rules
* how to generate your own log messages
* Using logrote

# Disk Management
* Partition
* MBR
* GPT
* Mount Points
* fdisk

-  Partition scheme
1. OS
2. Application
3. User
4. Swap

### MBR
* Master Boot record
* can only address 2 TB of disk space
* Being phased out by GPT
  1. GPT = GUID Partition Table
* 4 primary partitions
* Extended partitions allow you to create logical partitions.

### GPT
* GUID Partition Table, GUID = Global Unique Identifier
* Replacing the MBR Partitioning scheme
* Part of UEFI, UEFI is replacing BIOS
* Extended partitions allow you to create logical partitions
* Not supported on older OS, May require newer or special tools

### Mount Points
* A directory used to access the data on a partition
* /(slash) is always a mount point
* /home
* /home/jason is on the partition mounted on home

### file system
* ext = Extended filesystem
  1. ext2, ext3, and et4 are later realeases
  2. Often the default file system type

* Other file systems
   1. ReiserFs
   2. JFS
   3. XFS
   4. ZFS
   5. Btrfs

# LVM - Logical volume manager
* You can create file systems that extend across multiple storage devices.
* You can aggregate multiple storage devices intoa single loial volume.
* Expand or shrink file sysytems in real-time while the data remains online and fully accessible.
* Migrate data from one storage device to another while online.


### Logical volume creation process
1. Create one or more physical volumes
2. Create volume group from those one or more physical volumes.
3. Create one or more logical volumes from the volume group.

![Linux Directories](psvol.PNG?raw=true "Title")

* lvmdiskscan             //Shows all storage devices to use
* lsblk                   // more information
* lsblk -p
* fdisk -l                // see storage attached to the linux sysytem.
* eg : pv create /dev/sdb // create a Physical volume
* pvs                     // view the list of phy volume
* root > su -
* lvmdiskcscan || also to view the attached storage
* pvcreate /dev/sdb
* lvdisplay

### Extend the volume group
* vgextend vg_app /dev/sdc // to
* lvextend -L +5G -r /dev/vg_app  // increase the size of logical volume

### Creating LVs
* pvcreate /dev/sdb
* vgcreate vg_name /dev/sdb
* lvcreate -L 100G -n lv_name vg_name

### Extend logical vol.
* lvextend -L + 10G -r /dev/vg_name/lv_nam
* pvcreate /dev/sdc
* vgextend vg_name /dev/sdc

### LV remove cpmmand
* lvremove /dev/vg_name/lv_name
* vgreduce vg_name /dev/sdb
* vgremove vg_name