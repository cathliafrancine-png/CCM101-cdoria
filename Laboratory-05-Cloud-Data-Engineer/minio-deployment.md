# MinIO Deployment Documentation

## Technical Deployment Steps

MinIO was deployed using Docker inside the KillerCoda Ubuntu 24.04 Playground. The official `minio/minio` image was not accessible in the Playground, so the Bitnami Legacy MinIO image was used to successfully deploy the server.

### Docker Command Used

The following Docker command was used to deploy the MinIO server:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
bitnamilegacy/minio:2025.7.23-debian-12-r5
```

### Port Used

The MinIO Web Console was accessed using **port 9001**.

Port **9000** was used for the MinIO API, while port **9001** was used for the Web Console.

### Bucket Created

A bucket named **client-photos** was created through the MinIO Web Console.

A sample file named **Products.png** was uploaded to the `client-photos` bucket.

### Environment Variables

The `-e` flags in the Docker command define environment variables for the MinIO container.

* `MINIO_ROOT_USER=cloudadmin` sets the root administrator username used to log in to the MinIO Web Console.
* `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the root administrator password used for authentication.

These environment variables allow the MinIO server to be configured with administrator credentials when the container is started.
