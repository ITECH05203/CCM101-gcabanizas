# Laboratory 05 – Cloud Data Engineer

## Mission Overview

For this laboratory activity, I explored how cloud storage is used to store and manage different types of files, particularly images. I deployed an S3-compatible Object Storage server using MinIO and Docker within the KillerCoda environment. After setting up the server, I accessed the MinIO Web Console, created a bucket named `client-photos`, and uploaded a sample file to verify the storage system.

## Objectives

By completing this laboratory activity, I was able to:

* Understand the differences between Block, File, and Object Storage.
* Set up an S3-compatible Object Storage server using MinIO and Docker.
* Access a cloud storage service through a web interface using port forwarding.
* Create a storage bucket and upload files as objects.
* Record and document cloud storage procedures using Markdown.
* Add new cloud computing skills and activities to my professional GitHub portfolio.

## Tools Used

* KillerCoda Playground
* Docker
* MinIO
* GitHub
* Web Browser
* Markdown

## Skills Learned

## During this activity, I gained hands-on experience deploying MinIO through Docker and connecting to its Web Console using a web browser. I also practiced creating storage buckets and uploading files using Object Storage. Overall, the laboratory improved my understanding of cloud storage while giving me additional experience with Docker, Linux commands, and GitHub documentation.

# minio-deployment.md

# MinIO Deployment Documentation

## Docker Command Used

To deploy the MinIO Object Storage server, I used Docker within the KillerCoda Ubuntu environment. The following command was used successfully:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
quay.io/minio/minio server /data --console-address ":9001"
```

This command started a Docker container named `minio-server`. The MinIO image was obtained from `quay.io`.

## Port Used for Web Console

The MinIO Web Console was accessed through **port 9001** using the Traffic/Ports feature available in KillerCoda.

* **Port 9000** – MinIO API
* **Port 9001** – MinIO Web Console

## Bucket Name

The storage bucket created during the activity was:

**`client-photos`**

A sample file was uploaded to the bucket to confirm that the MinIO Object Storage server was properly configured and functioning.

## Environment Variables

The `-e` options in the Docker command define the environment variables used by MinIO.

* `MINIO_ROOT_USER=cloudadmin` – Defines the administrator username.
* `MINIO_ROOT_PASSWORD=CloudNova2026!` – Defines the administrator password.

These credentials are used to log in to the MinIO server and access its administrative features.

## Deployment Verification

To verify that the MinIO container was successfully running, I used:

```bash
docker ps
```

The output confirmed that the `minio-server` container was **Up** and that ports `9000` and `9001` were properly mapped.

