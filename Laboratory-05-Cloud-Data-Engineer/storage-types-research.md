# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type       | Description                                                                                                                                                            | Primary Use Case                                                                                                                           | Cloud Provider Example                 |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------- |
| **Block Storage**  | Stores data as fixed-size blocks that can be accessed individually. It is commonly attached to a virtual machine and functions similarly to a traditional hard drive.  | Best used for operating systems, databases, and applications that require low-latency storage and frequent read/write operations.          | **AWS Elastic Block Store (EBS)**      |
| **File Storage**   | Stores data in a hierarchical file and folder structure. Files can be shared and accessed by multiple systems through a network.                                       | Best used for shared file systems, documents, and applications that require files and folders to be accessed by multiple users or servers. | **Amazon Elastic File System (EFS)**   |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier. It is designed to store large amounts of unstructured data such as images, videos, and backups. | Best used for large-scale unstructured data, including user-uploaded images, videos, backups, and other files that need scalable storage.  | **Amazon Simple Storage Service (S3)** |

## Why Object Storage is Suitable for the Client

Object Storage is the best choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as user-uploaded images and can scale as the number of photos increases. It also allows the application to store files separately from the web server, making it suitable for a system that needs accessible and scalable storage for millions of images.
