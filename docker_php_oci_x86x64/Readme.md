Docker : PHP Env
***
## Image information
- Base Image : Ubuntu
- What will be installed
    - PHP 8.0
    - PHP Basic Extensions
    - OCI8
    - Oracle Instant Client(Basic, SDK)
***
## Warning
- **This Docker Image is only available to x86(64bit) CPU"**
- **Apple Sillicon, Linux ARM Platform supported**
- **This Docker Image support Oracle DB Connection**
***
## Run container
1. Build Container

```bash
docker build -t (image name) .
```

2. Run image

```bash
docker run -d -n (container name) -v (local volume directory):/var/www/html -p (local port):80 (image name)
```

3. Access URL

```text 
127.0.0.1:(local port)
```