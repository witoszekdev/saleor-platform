<div align="center">
  <h1>Saleor Platform - LOCAL DEVELOPMENT</h1>
</div>

<div align="center">
  <p>Run all Saleor services from one repository.</p>
  <p>This fork makes it easy to install apps that are running on <code>localhost</code> without creating a tunnel</p>
</div>

## About

This is a fork of official [`saleor-platform`](https://github.com/saleor/saleor-platform) that uses `host` network in `docker-compose.yaml` which makes installing apps locally possible.
Without this you would need to create reverse proxies inside Docker network or tunnels to make apps installable.

## Running it

```bash
docker compose up -d api worker
```

## Requirements

- Docker daemon that [supports `host` network](https://docs.docker.com/network/host/)
  - Linux: works out of the box
  - macOS: Docker Desktop is not supported, use [OrbStack](https://orbstack.dev/)
  - Windows: Docker Deksktop is not supported, no known solution at the moment

## License

Disclaimer: This repository is not affiliated or officially supported by Saleor Commerce
