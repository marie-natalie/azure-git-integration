# Azure Git Integration (CNS 3205)

An end-to-end implementation of an Ubuntu Linux virtual machine on Microsoft Azure integrated with Git and GitHub. This project demonstrates secure SSH key authentication, administrative user privilege management and automated scripting.

## What Was Done

* **Cloud VM Provisioning** — An Ubuntu Server instance running on Microsoft Azure.
* **User Management** — Dedicated user accounts with administrative privileges via the default `sudo` group.
* **SSH Key Setup** — Key-based authentication (`ed25519`) between local workstations, the Azure VM, and GitHub.
* **Repository** — A shared GitHub repository cloned to the server, initialized with a first commit and push.
* **Automation** — An `update.sh` script that generates content, stages, commits, and pushes updates in a single command.

## Standard Development Workflow

To push manual updates to the repository :
```bash
git add .
git commit -m "describe the change"
git push origin main
