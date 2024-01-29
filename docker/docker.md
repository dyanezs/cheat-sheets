# Docker Commands Cheat Sheet

## Pull Docker Images  
Pulls a Docker image from a registry. The optional tag specifies a version or variant of the image.

```bash
docker pull image-name[:tag]
```

## Build Images
Build a Docker image, specifying the Dockerfile path and build context:

```bash
docker build --no-cache -t your_image_name -f skynet/Dockerfile .
```

- `--no-cache`: Do not use the cache during the build process.
- `-t your_image_name`: Set a name for the built image.
- `-f skynet/Dockerfile`: Specify the path of the Dockerfile.
- `.`: Indicates the build context.

## List Images
List the Docker images on your local machine:

```bash
docker images
docker image ls
```

## View Running Images
See the currently running Docker containers:

```bash
docker ps
```

## Remove Images
Remove a Docker image by its ID:

```bash
docker image rm -f <image-id>
```

## Execute Images
Run a Docker container and enter its shell interactively:

```bash
docker run -it <image-id> bash
docker run -it --rm <image-id> bash  # Remove after exit
docker exec -it <image-id> bash
```
## Clean images
Remove All Unused Containers, Networks, and Volumes

```bash
docker system prune -a
```

## Colima Commands
When using Colima for Docker development:

```bash
colima start --network-address --vm-type qemu --runtime docker --cpu 4 --memory 4 --disk 64 --verbose
colima stop
colima list
```
