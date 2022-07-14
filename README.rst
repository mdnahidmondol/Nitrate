Nitrate - Test Case Management System
=====================================
## Step 1: Add Docker Repository in RHEL 8 
```sh
sudo dnf update sudo dnf install -y yum-utils 
```
```sh
sudo dnf config-manager –add-repo https://download.docker.com/linux/centos/docker-ce.repo
```
## Step 2: Update System Repositories 
```sh
sudo dnf update sudo dnf repolist
```
## Step 3: Remove Conflicting Packages
```sh
sudo dnf remove podman buildah
```
### Step 4: Install Docker on RHEL 8
```sh
sudo dnf install docker-ce docker-ce-cli containerd.io
```
### Step 5: Enable Docker Service
```sh
sudo systemctl start docker.service sudo systemctl enable docker.service sudo
```
```sh
systemctl status docker.service
```
## Step 6: Check Docker Version 
```sh
sudo docker version
```
full documentation https://bytexd.com/how-to-install-docker-on-rhel/

## Docker compose Installation

## Step 1: Install Curl command
```sh
sudo dnf install -y curl
```
## Step 2: Download the Docker Compose Binary 
```sh
sudo curl -L “https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)” -o /usr/local/bin/docker-compose
```
## Step 3: Change File permissions
```sh
sudo chmod +x /usr/local/bin/docker-compose
```
## Step 4: Verify Docker Compose Installation 
```sh
sudo docker-compose –version
```


full documentation https://bytexd.com/how-to-install-docker-compose-on-rhel-8-almalinux-rocky-linux/
# NEXT STEP
### clone this repo https://github.com/mdnahidmondol/Nitrate.git
```sh
git clone this repo https://github.com/mdnahidmondol/Nitrate.git
```
```sh
cd Nitrate
```

## Run docker-compose File
```sh
sudo docker-compose up -d
```
## Stop docker-compose
```sh
sudo docker-compose down
```