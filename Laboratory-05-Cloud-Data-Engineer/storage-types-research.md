
# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks that can be accessed individually. | Operating systems, databases, and virtual machine disks. | AWS EBS |
| File Storage | Stores data as files organized into folders and directories. | Shared files and applications that need a traditional file system. | AWS EFS |
| Object Storage | Stores data as objects together with metadata and a unique identifier. | Images, videos, backups, documents, and other unstructured data. | AWS S3 |

## Why Object Storage is Suitable for the Client

Object Storage is suitable for the client's photo-sharing application because it is designed for large amounts of unstructured data such as images. It can provide scalable storage while allowing applications to access individual files through an object-storage interface.
