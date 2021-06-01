# Amazon S3- Simple Storage Service

a scalable, high-speed, low-cost web-based service designed for online backup and archiving of data and application programs. It allows to upload, store, and download any type of files up to 5 TB in size.

- it is a storage for the Internet. It is designed to make web-scale computing easier. 

- it has a simple web services interface that you can use to store and retrieve any amount of data, at any time, from anywhere on the web. 

- it provides a highly scalable, reliable, fast, inexpensive data storage infrastructure


## Amazon S3 Advantages:

- Creating buckets 
- Creating buckets
- Downloading data 
- Permissions
- Standard interfaces 


## S3 concepts

- ## Buckets 
 a container for objects stored in Amazon S3.


buckets help:
- They organize the Amazon S3 namespace at the highest level.

- They identify the account responsible for storage and data transfer charges.

- They play a role in access control.

- They serve as the unit of aggregation for usage reporting.

- # Objects

 fundamental entities stored in Amazon S3. They consist of object data and metadata, 
 `data` --> is opaque to Amazon S3.
 `metadata` -->  is a set of name-value pairs that describe the object.

 Note: An object is uniquely identified within a bucket by a key (name) and a version ID 

 - # Keys
   a unique identifier for an object within a bucket. 
   Each object in a bucket has one key. 

- # Regions

You choose the geographical AWS Region where Amazon S3 will store the buckets that you create based on the latency,  costs, or regulatory requirements. 

Note: Objects stored in a Region never leave the Region unless you explicitly transfer them to another Region.  

## Amazon S3 data consistency model
Amazon S3 provides strong read-after-write consistency for PUTs and DELETEs of objects in your Amazon S3 bucket in all AWS Regions.
This applies to both writes to new objects as well as PUTs that overwrite existing objects and DELETEs

 Updates to a single key are atomic. 
 it achieves high availability by replicating data across multiple servers within AWS data centers.  

- A process writes a new object to Amazon S3 and immediately lists keys within its bucket. The new object will appear in the list.

- A process replaces an existing object and immediately tries to read it. Amazon S3 will return the new data.

- A process deletes an existing object and immediately tries to read it. Amazon S3 will not return any data as the object has been deleted.

- A process deletes an existing object and immediately lists keys within its bucket. The object will not appear in the listing.

## Amazon S3 features


- Storage classes
- Bucket policies
- AWS Identity and Access Management
- Access control lists
- Versioning
- Operations

## S3 with Amplify
 Amplify Storage category provides an interface for managing user content for your app in public, protected, or private storage buckets.

 The Storage category comes with default built-in support for Amazon Simple Storage Service (S3).  

 -  `Amplify CLI` helps you to create and configure the storage buckets for your app.

 - Install Amplify Libraries
 - Initialize Amplify Storage
 - Uploading data to your bucket
 














