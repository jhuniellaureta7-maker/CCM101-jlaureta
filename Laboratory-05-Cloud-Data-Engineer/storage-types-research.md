# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type   | Description                                                                                            | Primary Use Case                                                                            | Cloud Provider Example |
| -------------- | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------- | ---------------------- |
| Block Storage  | Stores data as individual blocks that can be attached to a virtual machine and used like a hard drive. | Best for operating systems, databases, and applications that require direct disk access.    | AWS EBS                |
| File Storage   | Stores data in files and folders that can be accessed through a shared file system.                    | Best for shared files, documents, and applications that need a common file system.          | AWS EFS                |
| Object Storage | Stores data as objects together with metadata and a unique identifier inside a storage system.         | Best for large amounts of unstructured data such as images, videos, backups, and documents. | AWS S3                 |

## Why Object Storage for User-Uploaded Images?

Object Storage is suitable for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as images. It allows uploaded photos to be stored as individual objects, making it appropriate for applications that need to manage many user-uploaded files.
