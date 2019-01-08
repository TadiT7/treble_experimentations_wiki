Here is a quick and dirty list of what are the changes in master/Q that impacts Treble:
- logical volumes (like LVM2 but re-made from scratch)
   - fastbootd (a SECOND fastboot, which will run inside recovery)
   - dynamically resizable/deletable/creatable partitions
   - does it include userdata?
- gsid. Systems will be able to boot GSI instead of themselves
   - GSIs will be "flashable" from (rooted?) shell ( https://android-review.googlesource.com/c/platform/system/gsid/+/863812 )
   - there will be a separated userdata_gsi partition ( https://android-review.googlesource.com/c/platform/system/core/+/863889 )