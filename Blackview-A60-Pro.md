# Blackview A60 Pro

Cheap and Cheerful

AOSP/GSI works perfectly well


## Unlock bootloader

1. Enable developer mode 
2. OEM unlock

## Download files

All credits to: https://www.youtube.com/watch?v=m6lvYCMflX8

1. recovery.img

2. vbmeta.img

3. your favorite gsi - use only - treble_arm64_bvN ARM 64-bit, AB (64bit) examples:
	
	```system-quack-arm64-ab-vanilla.img```
	```lineage-17.1-20200607-UNOFFICIAL-treble_arm64_bvN```

## Now in a terminal or cmd

```bash
user@linux: ~/Downloads/blackview $ fastboot devices
A60ProEEA0039042	fastboot
user@linux: ~/Downloads/blackview $ fastboot flashing unlock
                                                   FAILED (remote: 'unknown command')
fastboot: error: Command failed
user@linux: ~/Downloads/blackview $ fastboot oem unlock
                                                   FAILED (remote: 'unknown command')
fastboot: error: Command failed
user@linux: ~/Downloads/blackview $ fastboot oem unlock
                                                   FAILED (remote: 'unknown command')
fastboot: error: Command failed
user@linux: ~/Downloads/blackview $ fastboot oem unlock
                                                   FAILED (remote: 'unknown command')
fastboot: error: Command failed
user@linux: ~/Downloads/blackview $ fastboot 
fastboot: usage: no command
user@linux: ~/Downloads/blackview $ fastboot oem
fastboot: usage: empty oem command
user@linux: ~/Downloads/blackview $ fastboot oem help
                                                   FAILED (remote: 'unknown command')
fastboot: error: Command failed
user@linux: ~/Downloads/blackview $ fastboot oem 
fastboot: usage: empty oem command
user@linux: ~/Downloads/blackview $ fastboot unlock
fastboot: usage: unknown command unlock
user@linux: ~/Downloads/blackview $ fastboot oem unlock-go
                                                   FAILED (remote: 'unknown command')
fastboot: error: Command failed
user@linux: ~/Downloads/blackview $ fastboot flashing unlock
                                                   (bootloader) Start unlock flow

OKAY [ 26.867s]
Finished. Total time: 26.867s
user@linux: ~/Downloads/blackview $ ls
deviceinfo.png	README	recovery.img  trebleinfo-blackview-a60-pro.png	v-220-system-quack-arm64-ab-vanilla.img  vbmeta.img
user@linux: ~/Downloads/blackview $ fastboot --disable-verification flash vbmeta  vbmeta.img
Rewriting vbmeta struct at offset: 0
Sending 'vbmeta' (4 KB)                            OKAY [  0.007s]
Writing 'vbmeta'                                   OKAY [  0.002s]
Finished. Total time: 0.012s
user@linux: ~/Downloads/blackview $ cat README 
To unlock oem type
  
fastboot devices
fastboot flashing unlock
or fastboot oem unlock

To Install Recovery

fastboot devices
fastboot --disable-verification flash vbmeta vbmeta.img
fastboot flash recovery recovery.img

user@linux: ~/Downloads/blackview $ ls
deviceinfo.png	README	recovery.img  trebleinfo-blackview-a60-pro.png	v-220-system-quack-arm64-ab-vanilla.img  vbmeta.img
user@linux: ~/Downloads/blackview $ fastboot flash recovery  recovery.img
Sending 'recovery' (32768 KB)                      OKAY [  1.633s]
Writing 'recovery'                                 OKAY [  0.812s]
Finished. Total time: 2.447s
user@linux: ~/Downloads/blackview $ fastboot erase system
******** Did you mean to fastboot format this ext4 partition?
Erasing 'system'                                   OKAY [  0.494s]
Finished. Total time: 0.495s
user@linux: ~/Downloads/blackview $ fastboot flash system v
v-220-system-quack-arm64-ab-vanilla.img  vbmeta.img                               
user@linux: ~/Downloads/blackview $ fastboot flash system v-220-system-quack-arm64-ab-vanilla.img 
Sending sparse 'system' 1/13 (131068 KB)           OKAY [  6.364s]
Writing 'system'                                   OKAY [  3.218s]
Sending sparse 'system' 2/13 (131068 KB)           OKAY [  7.433s]
Writing 'system'                                   OKAY [  3.228s]
Sending sparse 'system' 3/13 (130676 KB)           OKAY [  6.326s]
Writing 'system'                                   OKAY [  3.213s]
Sending sparse 'system' 4/13 (131068 KB)           OKAY [  6.360s]
Writing 'system'                                   OKAY [  3.215s]
Sending sparse 'system' 5/13 (130664 KB)           OKAY [  6.335s]
Writing 'system'                                   OKAY [  3.205s]
Sending sparse 'system' 6/13 (131068 KB)           OKAY [  6.298s]
Writing 'system'                                   OKAY [  3.214s]
Sending sparse 'system' 7/13 (130664 KB)           OKAY [  6.268s]
Writing 'system'                                   OKAY [  3.199s]
Sending sparse 'system' 8/13 (131068 KB)           OKAY [  6.301s]
Writing 'system'                                   OKAY [  3.217s]
Sending sparse 'system' 9/13 (130664 KB)           OKAY [  6.273s]
Writing 'system'                                   OKAY [  3.204s]
Sending sparse 'system' 10/13 (131068 KB)          OKAY [  6.360s]
Writing 'system'                                   OKAY [  3.214s]
Sending sparse 'system' 11/13 (131068 KB)          OKAY [  6.372s]
Writing 'system'                                   OKAY [  3.214s]
Sending sparse 'system' 12/13 (130744 KB)          OKAY [  6.318s]
Writing 'system'                                   OKAY [  3.202s]
Sending sparse 'system' 13/13 (124564 KB)          OKAY [  6.323s]
Writing 'system'                                   OKAY [  3.063s]
Finished. Total time: 124.942s
user@linux: ~/Downloads/blackview $ fastboot -w
Erasing 'userdata'                                 OKAY [  0.388s]
mke2fs 1.45.4 (23-Sep-2019)
Creating filesystem with 2562555 4k blocks and 640848 inodes
Filesystem UUID: c19b441c-95ec-463b-bfc9-d1929a0af72d
Superblock backups stored on blocks: 
	32768, 98304, 163840, 229376, 294912, 819200, 884736, 1605632

Allocating group tables: done                            
Writing inode tables: done                            
Creating journal (16384 blocks): done
Writing superblocks and filesystem accounting information: done 

Sending 'userdata' (116 KB)                        OKAY [  0.013s]
Writing 'userdata'                                 OKAY [  0.035s]
Erasing 'cache'                                    OKAY [  0.019s]
mke2fs 1.45.4 (23-Sep-2019)
Creating filesystem with 110592 4k blocks and 110592 inodes
Filesystem UUID: 4d499de5-e4be-4583-9941-f2de7e1da915
Superblock backups stored on blocks: 
	32768, 98304

Allocating group tables: done                            
Writing inode tables: done                            
Creating journal (4096 blocks): done
Writing superblocks and filesystem accounting information: done

Sending 'cache' (68 KB)                            OKAY [  0.010s]
Writing 'cache'                                    OKAY [  0.021s]
Erasing 'metadata'                                 OKAY [  0.008s]
Erase successful, but not automatically formatting.
File system type raw data not supported.
Finished. Total time: 0.551s
k
```

## Screenshots

### Before
![alt text](https://raw.githubusercontent.com/sale2000/blackviewa60pro/master/deviceinfo.png "Device info")

