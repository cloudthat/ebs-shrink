ebs-shrink
==========
Amazon’s Elastic Block Store Volumes are easy to use and expand but notoriously hard to shrink once their size has grown. Here is Script for Shrinking any Mounted EBS Volume on EC2 Instances

This Script Assumes that one or More EBS Volumes is Mounted on the  EC2 Instance

This Script Will Create a New Volume of User Defined,Mount it to /mnt/ebs1 Copy all the data from the attached EBS Volume recursively that need to be Migrated  preserving all the user permissions,then Unmount it and Mount the Newly Created EBS Volume at the Same Mount Point

Note:The Migrated Volume is Not Deleted it is just Unmounted  So if any error occurs we can reattach it.
     This Script can only use for Attached(Mounted) EBS Volumes not Root Volume.
     
       
