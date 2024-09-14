# Docker File

## Docker Production Development - Dockerfile

First, build the image by opening the terminal in the project's root directory.

```bash
docker buildx build . -t headless-commerce:latest
```

Run the image and specify port mapping with the `-p` flag.

```bash
docker run --rm -it -p 9000:9000 headless-commerce:latest
```

## Docker Production Build - Dockerfile.prod

First, build the image by opening the terminal in the project's root directory.

```bash
docker buildx build . -t headless-commerce:latest -f Dockerfile.prod
```

Run the image and specify port mapping with the `-p` flag.

```bash
docker run --rm -it -p 9000:9000 headless-commerce:latest
```