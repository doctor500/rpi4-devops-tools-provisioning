# RPi 4 DevOps Tools Provisioning
Just a repository for provision DevOps tools in Docker RPi4

![Lines of code](https://img.shields.io/tokei/lines/github/doctor500/rpi4-devops-tools-provisioning?style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/doctor500/rpi4-devops-tools-provisioning?style=for-the-badge)

Ready to deploy tools list:
![Jenkins Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Jenkins_logo_with_title.svg/1280px-Jenkins_logo_with_title.svg.png)

# Folder Content
```
📦rpi4-devops-tools-provisioning
┣📂jenkins   
┃ ┣📂configuration
┃ ┃ ┗ 📜casc.yaml
┃ ┣📂data
┃ ┃ ┗📂drive
┃ ┃   ┗📂jenkins
┃ ┣📜docker-compose.yml
┃ ┣🐳Dockerfile
┃ ┗🧾plugins.txt 
┃ 
┗🧾README.md
```

# Jenkins
Key features
- Latest LTS version
- Ready to use / less config (JCasC)

## Quick Start
Go inside `jenkins` folder and run the docker compose command
```bash
cd ./jenkins
```
```bash
docker-compose --context yourRpiContextName up -d
```
change `yourRpiContextName` with your context name. you can see [wiki section](https://github.com/doctor500/rpi4-devops-tools-provisioning#installation-guide-tips--trick) to setup your docker context.

## Update/Reload Config `casc.yaml`
The configuration in `casc.yaml` will not change immediately when you update this file. If you want to update, you can enter the menu **Manage Jenkins** > **Configuration as Code** and click **Reload existing configuration** button


# Installation Guide, Tips & Trick

Checkout [this repo wiki](https://github.com/doctor500/rpi4-devops-tools-provisioning/wiki) section to get effective guides or Docker operation tips from Raspberry Pi 4