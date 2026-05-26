# Kubernetes Local Dev Environment Installer

A simple Ubuntu setup script to install:

- Docker
- Kind (Kubernetes in Docker)
- kubectl

Perfect for quickly setting up a local Kubernetes development environment on Ubuntu machines.

---

## Features

- Automatic installation of Docker, Kind, and kubectl
- Supports both `x86_64` and `ARM64`
- Skips already installed components
- Configures Docker permissions automatically
- Simple one-command setup

---

## Prerequisites

- Ubuntu machine
- `curl` installed
- `sudo` access

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

### Make Script Executable

```bash
chmod +x install.sh
```

### Run the Script

```bash
./install.sh
```

> If Docker was newly installed, run:
>
> ```bash
> newgrp docker
> ```
>
> or log out and log back in.

---

## Verify Installation

```bash
docker --version
kind --version
kubectl version --client
```

---

## Installed Tools

## License
MIT License

---
- `ARM64 / aarch64`

- `x86_64`
| Tool | Purpose |


## Supported Architectures
|---|---|
---

