# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type       | Description                                                                                            | Primary Use Case                                                                                   | Cloud Provider Example |
| ------------------ | ------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------- | ---------------------- |
| **Block Storage**  | Divides data into fixed-size blocks that can be accessed and managed similar to a physical hard drive. | Suitable for virtual machines, databases, and applications that require high-speed storage.        | AWS EBS                |
| **File Storage**   | Organizes data into files and folders that can be accessed and shared through a network.               | Ideal for shared documents, files, and applications that require a common file system.             | AWS EFS                |
| **Object Storage** | Saves data as individual objects along with metadata that provides information about each object.      | Well-suited for storing large amounts of unstructured data, including photos, videos, and backups. | AWS S3                 |

## Why Object Storage is Best for the Client

Object Storage is the most suitable option for the client's photo-sharing application because it is specifically designed to handle large volumes of unstructured data, such as images. It allows uploaded files to be organized into buckets and objects, making it easier to store and manage a large number of photos. Because of its scalability, it can support an application that may eventually need to store millions of images.

