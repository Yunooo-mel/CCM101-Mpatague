# Research: Types of Cloud Storage

## Comparison Table

| Storage Type | Description (How does it store data?) | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Splits data into fixed-size blocks, each with its own address. Acts like a raw hard drive attached to a single server. | Operating systems, databases, and apps needing fast, low-latency reads/writes. | AWS EBS, Azure Managed Disks, Google Persistent Disk |
| **File Storage** | Stores data as files in a folder hierarchy (directories and paths). Shared over a network so multiple machines can access it at once. | Shared drives, home directories, content management, team collaboration. | AWS EFS, Azure Files, Google Filestore |
| **Object Storage** | Stores data as objects in a flat structure. Each object holds the data, metadata, and a unique ID. Accessed over HTTP/API. | Images, videos, backups, logs, and other massive unstructured data. | AWS S3, Azure Blob Storage, Google Cloud Storage |

## Why Object Storage for the Client's Photos

Object Storage is the best choice because it scales almost without limit, so millions of user-uploaded images can be stored without managing disks or capacity. It is also cost-effective and accessible from anywhere through a simple web API, and it keeps images outside the temporary web server container. Built-in metadata and replication also keep the photos organized and durable.
