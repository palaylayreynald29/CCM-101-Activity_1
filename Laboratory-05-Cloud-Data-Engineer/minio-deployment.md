
# MinIO Deployment

## Deployment Overview

For this laboratory activity, I deployed MinIO using Docker. MinIO provides an S3-compatible object storage service that can be accessed through a web console.

## Docker Command

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
