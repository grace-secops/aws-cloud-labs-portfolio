 AWS EBS Storage Lab

 Objective

To configure Amazon Elastic Block Store (EBS) and understand how persistent block storage can be attached to and used with an Amazon EC2 instance.

The purpose of this exercise was to gain practical experience creating, formatting, mounting, and backing up an EBS volume.

 AWS Services

* Amazon EC2
* Amazon EBS

 Lab Environment

* AWS Management Console
* Controlled AWS lab environment
* AWS Region: US East (N. Virginia)

 EBS Volume Creation

A new EBS volume was created and attached to an EC2 instance.

The volume was prepared for use as additional persistent storage separate from the instance's root volume.

 Volume Formatting

The attached EBS volume was formatted using the ext3 file system.

This prepared the volume to store and manage files within the Linux environment.

 Mounting the EBS Volume

The EBS volume was mounted to:

```text
/mnt/data-store
```

This allowed the additional storage to be accessed through the specified directory.

 Persistent Mount Configuration

The system's `/etc/fstab` configuration was updated so that the EBS volume could be mounted persistently.

This configuration helps ensure that the storage remains available after a system restart.

 EBS Snapshot

A snapshot of the EBS volume was created.

The snapshot was then used to demonstrate the process of restoring storage from a point-in-time backup.

This provided practical experience with an important AWS storage backup and recovery mechanism.

 Key Learning

This exercise helped me understand how EBS provides persistent block storage for EC2 instances.

I gained practical experience creating an EBS volume, formatting it, mounting it to a Linux directory, configuring persistent mounting, and using snapshots for backup and recovery.

 Security and Availability Considerations

EBS volumes may contain sensitive application or system data, so appropriate access controls should be applied.

Regular snapshots can also provide an additional recovery option in the event of data loss or infrastructure failure.

 Conclusion

The EBS lab provided practical experience managing persistent cloud storage in AWS.

The exercise reinforced the relationship between EC2 compute resources and EBS storage and demonstrated how snapshots can support backup and recovery strategies.
