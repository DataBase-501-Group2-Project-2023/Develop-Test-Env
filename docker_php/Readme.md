Docker : PHP Env
***
## Image information
- Base Image : php, latest
***
## Run container
1. Build Container

```bash
docker build -t (image name) .
```

2. Run image

```bash
docker run -d --name (container name) -v (local volume directory):/var/www/html -p (local port):80 (image name)
```

3. Access URL

```text
127.0.0.1:(local port)
```
