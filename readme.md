# ngnix

An nginx image with Brotli and Headers More built into it. Based on [fholzer/docker-nginx-brotli](https://github.com/fholzer/docker-nginx-brotli), [nginx](https://www.nginx.com/), [Brotli module](https://github.com/google/ngx_brotli) and [Headers More module](https://github.com/openresty/headers-more-nginx-module).

# Documentation

- [Nginx](https://nginx.org/en/docs/)
- [Brotli](https://github.com/google/ngx_brotli#configuration-directives)
- [Headers More](https://github.com/openresty/headers-more-nginx-module#version)

# Build

```bash
$ docker buildx create --name nginx --platform linux/amd64,linux/arm64
$ docker buildx use nginx
$ docker buildx build --push --platform linux/amd64,linux/arm64 --file Dockerfile --tag yoohahn/nginx:latest .
$ docker buildx build --push --platform linux/amd64,linux/arm64 --file Dockerfile --tag yoohahn/nginx:VERSION .
```
