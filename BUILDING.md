Ensure buildx/BuildKit support is enabled and run:

```shell script
docker buildx build --platform=linux/arm64 --platform=linux/arm/v7 --platform=linux/amd64 --tag tekn0ir/minecraft-server:multiarch --push .
docker buildx build --platform=linux/arm64 --tag tekn0ir/minecraft-server:arm64 --push .
```

To build for local testing, use:

```shell script
docker buildx build --platform=linux/amd64 --tag mc-multiarch --load .
```
