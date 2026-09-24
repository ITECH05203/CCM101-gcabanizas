# MinIO Deployment

## Docker Command Used

I used the following Docker command to deploy the MinIO server:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" bitnamilegacy/minio:latest
```

The container was successfully created and started with the name `minio-server`.

## Web Console Port

The MinIO Web Console uses **port 9001**. Port 9000 is used for the MinIO API.

The Docker port mapping was:

```text
9000:9000
9001:9001
```

## Bucket Name

The bucket I created is:

**client-photos**

## Environment Variables

The `-e` flags were used to set the environment variables for the MinIO administrator login credentials.

* `MINIO_ROOT_USER=cloudadmin` sets the username for the administrator account.
* `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the password for the administrator account.

These environment variables allow the MinIO server to start with the specified administrator credentials.

