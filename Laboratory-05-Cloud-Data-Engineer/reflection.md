# Mission Reflection

This laboratory helped me understand how object storage can be used to manage large amounts of data, especially files such as photos. Object storage is better suited for storing millions of photos because it is designed to store individual objects together with their metadata. Unlike traditional block storage, object storage can organize and manage large amounts of unstructured data through buckets, making it practical for applications that need to store many files.

Using Docker also made deploying the MinIO storage server easier. Instead of manually installing and configuring every component, I was able to download a MinIO container image and run the server using a Docker command. The environment variables allowed me to configure the administrator username and password, while the port mappings allowed me to access the MinIO Web Console through a browser. This made the deployment process more organized and repeatable.

A bucket in cloud storage is a container used to organize and store objects such as images, documents, and other files. In this laboratory, I created a bucket named `client-photos` and uploaded a sample image into it. This demonstrated how files can be stored and managed using an object storage system.

Large enterprise companies can protect their object storage data from physical server failures by maintaining multiple copies of data and storing them across different servers or locations. They can also use backups, redundancy, replication, and other recovery mechanisms to reduce the risk of permanent data loss when hardware fails.

My confidence in navigating the Linux command line is also growing. At first, some Docker and Linux commands were unfamiliar to me, especially when errors occurred. However, by checking the command output, correcting mistakes, and successfully deploying MinIO, creating a bucket, and uploading a file, I became more comfortable using the terminal. This laboratory gave me practical experience with Linux, Docker, and object storage.
