# Kubernetes Local Dev Environment Installer

A lightweight and reliable shell script to automate the installation of:

- Docker
- Kind (Kubernetes in Docker)
- kubectl

on Linux systems.

The script automatically detects system architecture (`x86_64` and `ARM64`) and downloads the correct binaries for a smooth setup experience.

---

## Features

- ✅ Automated dependency checks  
  Skips components that are already installed.

- ✅ Multi-Architecture Support  
  Supports:
  - `x86_64` (Intel/AMD)
  - `aarch64` / `arm64` (ARM-based systems)

  Ideal for:
  - Local development machines
  - Cloud environments such as AWS EC2 Graviton instances

- ✅ Docker Permission Configuration  
  Automatically adds the current user to the `docker` group.

- ✅ Robust Error Handling  
  Uses:
  ```bash
  set -e
  set -o pipefail
  ```

  to stop execution immediately if any step fails.

---

## Prerequisites

Before running the script, ensure you have:

- A Linux environment  
  *(Ubuntu/Debian-based distributions are recommended for Docker installation support)*

- `curl` installed

- `sudo` privileges

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

```
---
### 3. Run the Script
```bash
> **Note:**  
> (or run `newgrp docker`) for Docker group permissions to take effect.
This allows you to run Docker and Kind commands without using `sudo`.
---

## What This Script Installs

### Docker


---


A tool for running local Kubernetes clusters using Docker containers as nodes.

---


The Kubernetes command-line utility used to:

- Deploy applications
- Inspect resources
- Manage Kubernetes clusters

---

## Verification

At the end of the installation, the script automatically prints the installed versions.

You can also verify them manually:

```bash
docker --version
kind --version
kubectl version --client --output=yaml
```

---

## Supported Architectures

| Architecture | Supported |
|---|---|
| x86_64 | ✅ |
| ARM64 / aarch64 | ✅ |

---

## Example Use Cases

- Local Kubernetes development
- Learning Kubernetes
- CI/CD practice environments
- AWS EC2 Kubernetes sandbox setup
- Docker + Kubernetes testing labs

---

## License

This project is open-source and available under the MIT License.

---

## Contributing

Contributions, issues, and feature requests are welcome.

Feel free to fork the repository and submit a pull request.

---

## Author

Developed for simplifying Kubernetes local environment setup on Linux systems.### kubectl
### Kind
The container runtime engine used by Kind to create Kubernetes nodes.


> If Docker was freshly installed, you must log out and log back in  

```
./install.sh



---
chmod +x install.sh

### 2. Make the Script Executable
```bash

