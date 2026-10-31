# Docker NGINX Demo

A simple static web page served by NGINX inside a Docker container.

## Run locally

```bash
docker build -t docker-nginx-demo .
docker run -d -p 8080:80 --name docker-nginx-demo docker-nginx-demo
```

Then open:

```text
http://localhost:8080
```

## Files

- `index.html` — the page content
- `Dockerfile` — container build instructions

## Description

This project demonstrates the flow:

```text
Dockerfile -> Image -> Container -> NGINX web server
```
