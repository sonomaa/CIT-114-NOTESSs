# Notes 7: Storage

## What is Storage?
- Storage is basically a technology that allows a user to retain digital data onto a medium. 
### Volatile vs Non-Volatile
- Volatile memory is a type of storage whose contents are erased when the system's power is turned off or interrupted. For example, RAM is volatile.
- Non-volatile memory is a term used to describe any memory or storage that is saved regardless of the power to the computer is on or off. ie. ROM
### Read Only Memory (RAM)
- As the computer boots, parts of the operating system and drivers are loaded into memory (RAM), which allows the CPU to process the instructions faster and speeds up the boot process. RAM is temporary storage that allows data and programs to be stored in memory in order the operating system to use them.
### Hard Drives
- A hard drive can be used to store any data, including pictures, music, videos, text documents, and any files created or downloaded. 
## Disaster Recovery and Technology
- In order to make decisions on how you will manage storage infrastructure, it is important to understand some key concepts from disaster recovery and how that will impact your decisions in traditional and cloud storage infrastructure.
### Disaster Recovery
- Disaster recovery (DR) starts with a plan that works in conjunction with the business continuity and contingency plans.  first step in recovering from a disaster is making sure that the disaster is over. 
### Fault Tolerance 
- Fault tolerance is the idea that a system can continue to run properly even in the event of a failure of a component of that system. 
### Replication
- In terms of data, replicated data is written to multiple hard drives possibly in multiple locations.
### Redundancy
-  The infrastructure may not be identical nor powerful enough to run on for a long period of time, but it will be good enough to run a business while the problem that caused the failure is identified and fixed.

## Storage in the Enterprise

### Redundant Array of Independent Disks (RAID)
- Computers and servers can use a RAID to replicate data across multiple redundant drives in order to ensure data is available. RAIDs are used often as part of other devices such as Network Attached Storage, Storage Area Networks, as well as internal drives for a Computer or File Server.
### File Servers
- A file server is a type of server on a network that is used to provide authorized users with access to files. It has all of the same components that a computer or server has including a CPU, RAM and storage, but the storage used for serving files is generally larger and optimized for serving files.
### Network Attached Storage (NAS)
- A NAS device is any storage device that is connected to a network and provides a network with additional storage. A NAS does not have any processing power on its own, meaning it cannot be used to execute or run network shared programs
### Storage Area Network (SAN) 
-  specialized high-speed network that provides access at a raw block-address level. 

## Storage in the Cloud
- This gives you agility, global scale and durability, with “anytime, anywhere” data access.
- Cloud storage uses many of the same technologies as Enterprise IT storage solutions, but at a significantly larger scale
### How Does Cloud Storage Work?
- Cloud storage is purchased from a third party cloud vendor who owns and operates data storage capacity and delivers it over the Internet in a pay-as-you-go model. These cloud storage vendors manage capacity, security and durability to make data accessible to your applications all around the world.
### Benefits of Cloud Storage
- Total Cost of Ownership: With cloud storage, there is no hardware to purchase, storage to provision, or capital being used for "someday" scenarios. 
- Time to Deployment:When development teams are ready to execute, infrastructure should never slow them down.
- Information Management : Centralizing storage in the cloud creates a tremendous leverage point for new use cases. 

### Cloud Storage Requirements
- Durability. Data should be redundantly stored, ideally across multiple facilities and multiple devices in each facility. 
- Availability. All data should be available when needed, but there is a difference between production data and archives.
- Security. All data is ideally encrypted, both at rest and in transit.
### Types of Cloud Storage
- Object Storage: Object storage solutions are ideal for building modern applications from scratch that require scale and flexibility, and can also be used to import existing data stores for analytics, backup, or archive.
- File Storage : . This type of storage is often supported with a Network Attached Storage (NAS) server. File storage solutions are ideal for use cases like large content repositories
- Block Storage :  Block-based cloud storage solutions are provisioned with each virtual server and offer the ultra low latency required for high performance workloads.
## Five Ways to Use Cloud Storage

### Backup and Recovery
-  Embedded data management policies like Amazon S3 Object Lifecycle Management can automatically migrate data to lower-cost tiers based on frequency or timing settings, and archival vaults can be created to help comply with legal or regulatory requirements. These benefits allow for tremendous scale possibilities within industries such as financial services, healthcare, and media that produce high volumes of data with long-term retention needs.
### Software Test and Development 
- Software test and development environments often requires separate, independent, and duplicate storage environments to be built out, managed, and decommissioned.
### Cloud Data Migration 
- Cloud data migration services services such as AWS Import/Export Snowball an simplify migrating storage into the cloud by addressing high network costs, long transfer times, and security concerns.
### Compliance
-  Cloud data compliance controls like Amazon Glacier Vault Lock are designed to ensure that you can easily deploy and enforce compliance controls on individual data vaults via a lockable policy. 
### Big Data and Data Lakes
-  Big data projects demand large-scale, affordable, highly available, and secure storage pools that are commonly referred to as data lakes.

## Encrypting Storage
- Encryption is a method securing data by taking data and making it unreadable without the right decryption information.
### Plain Text vs. Cipher Text
- Plain text is the original message or information before it has been encrypted. This text can be read by anyone as it is readable text.
- Cipher text is the encrypted version of the original plain text message after algorithm called a cipher has been applied to it. The encryption algorithm takes the plain text message and makes it so that it is no longer readable text.
### Data at Rest
- Data at rest simply means that the information is being stored physically where it is inactive or in use but not in being actively transmitted over a network. This data is most at risk for being stolen via physical theft or unauthorized access to file storage.
### Data in Transit
- Data encryption while files are in transit is different that encryption at rest. When a file is in transit, you have two or more computers involved. 
## Backup Locations
### Stored Locally
- Backups that are stored locally generally use an external hard drive, RAID, network attached storage (NAS), USB drive or even a DVD, where the backup is in the same physical location (on-site) as the business.
### Cloud Storage
- Cloud storage allows for a business to move the backup to cloud storage infrastructure outside of the business location. Saving important data to cloud storage such as Google Drive, Dropbox, or Box.com can help move data outside away from the local business. This is great for easy always on access where you can modify files directly in those solutions. 
### Onsite vs Off-site
- An on-site backup is the kind that is physically kept at the business site, generally local storage. They can be a secondary hard drive, a USB drive
- An off-site backup is exactly as it sounds, it is stored physically away from the business. This type of backup is becoming more popular with cloud-based backup solutions.

## What are the core AWS Storage Services?
- There are three core types of cloud storage that AWS and other cloud providers support: Object Storage, File Storage, and Block Storage. Within each of these types, are specific services that provide storage within the AWS Intrastructure.
## Amazon Simple Storage Service (Amazon S3)
- fully managed object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. 
## Amazon S3 Glacier
-  is a secure, durable, and extremely low-cost storage service for data archiving and long-term backup. It is designed to deliver 99.999999999% durability. 
##  Amazon Elastic File System (Amazon EFS)
-  a simple, scalable, elastic file system for Linux-based workloads for use with AWS Cloud services and on-premises resources. It is built to scale on demand to petabytes without disrupting applications, growing and shrinking automatically
-Amazon EFS is a fully managed service that requires no changes to your existing applications and tools, providing access through a standard file system interface for seamless integration.
##  Amazon Elastic Block Store
- Block storage solutions are typically faster and use less bandwidth, but they can cost more than object-level storage.
## Introduction to Static Web Hosting
- You can easily and inexpensively use Amazon Web Services (AWS) to host a website that uses client-side technologies (such as HTML, CSS, and JavaScript) and does not require server-side technologies (such as PHP and ASP.NET). This type of site is called a static website, and is used to display content that does not change frequently. 

### Interesting Quotes. 
- " It(Amazon EFS) is built to scale on demand to petabytes without disrupting applications, growing and shrinking automatically as you add and remove files, so your applications have the storage they need – when they need it"
- " Elastic Volumes allows you to dynamically increase capacity, tune performance, and change the type of any new or existing current generation volume with no downtime or performance impact. Easily right-size your deployment and adapt to performance changes." 

### New Facts: 
-  Volatile memory is a type of storage whose contents are erased when the system's power is turned off or interrupted. For example, RAM is volatile.
- Non-volatile memory is a term used to describe any memory or storage that is saved regardless of the power to the computer is on or off. ie. ROM


