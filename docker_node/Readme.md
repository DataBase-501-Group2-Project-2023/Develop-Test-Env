Docker : Node Env
***
## Image information
- Base Image : Node, latest
- Volume
    - /backend : project directory
- Port Expose
    - 3000 : Swagger Documentation
    - 4000 : Project Port
***
## Run container
1. Build Container

```bash
docker build -t (image name) .
```

2. Run image

```bash
docker run -itd --rm --name (container name) -v (local mount volume):/backend -p (local port):3000 -p (local port):4000 (image name) bash
```

3. Get into container

```bash
# With default terminal
docker attach (container name)

# With new env shell
docker exec -it (container name) bash
```
