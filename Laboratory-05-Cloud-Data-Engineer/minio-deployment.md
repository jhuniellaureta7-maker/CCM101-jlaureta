# MinIO Object Storage Deployment

## Deployment Command

The following command was executed to pull and run the MinIO server container:

\`\`\`bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  quay.io/minio/minio server /data --console-address ":9001"
\`\`\`

**Note:** The image `quay.io/minio/minio` was used instead of `minio/minio` since MinIO's image is no longer distributed through Docker Hub. Attempting to pull `minio/minio` results in a "pull access denied" error, so quay.io is now the correct source for the official image.

## Port Mapping

| Port | Purpose            |
|------|---------------------|
| 9000 | MinIO API endpoint   |
| 9001 | MinIO Web Console    |

The web console was reached by opening port **9001** through KillerCoda's Traffic/Ports panel.

## Understanding the Environment Variables

Two `-e` flags were passed into the container at runtime:

- `MINIO_ROOT_USER=cloudadmin` — defines the administrator username required to authenticate into the MinIO console and API.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` — defines the administrator password paired with the root user for login access.

Passing credentials this way keeps them configurable per deployment rather than hardcoded into the container image, which is a more secure and flexible approach.

## Confirming the Deployment

Once the container started, its status was checked with:

\`\`\`bash
docker ps
\`\`\`

The container appeared as `minio-server` with a status of "Up," confirming that both ports were correctly bound and the service was running.

## Bucket and Upload

Through the MinIO Web Console, a new bucket named **client-photos** was created to represent the storage location for the client's user-uploaded images. A sample file was then uploaded into this bucket to confirm that the object storage server was fully functional and reachable.

## Screenshot Evidence

| File | Description |
|------|--------------|
| `screenshots/minio-deployed.png` | Terminal output showing the successful container deployment |
| `screenshots/minio-bucket-upload.png` | MinIO console showing the created bucket and uploaded file |
