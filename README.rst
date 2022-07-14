Nitrate - Test Case Management System
=====================================


$ sudo dnf config-manager --add-repo=https://download.docker.com/linux/centos/docker-ce.repo


sudo dnf repolist -v
### Step 1: Add Docker Repository in RHEL 8
sudo dnf update
sudo dnf install -y yum-utils
sudo dnf config-manager –add-repo https://download.docker.com/linux/centos/docker-ce.repo


### Step 2: Update System Repositories
sudo dnf update
sudo dnf repolist

### Step 3: Remove Conflicting Packages
sudo dnf remove podman buildah


### Step 4: Install Docker on RHEL 8

sudo dnf install docker-ce docker-ce-cli containerd.io

### Step 5: Enable Docker Service

sudo systemctl start docker.service
sudo systemctl enable docker.service
sudo systemctl status docker.service

### Step 6: Check Docker Version
sudo docker version


https://bytexd.com/how-to-install-docker-on-rhel/


### Docker compose Installation


### Step 1: Install Curl command

sudo dnf install -y curl


### Step 2: Download the Docker Compose Binary
sudo curl -L “https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)” -o /usr/local/bin/docker-compose

### Step 3: Change File permissions

sudo chmod +x /usr/local/bin/docker-compose

### Step 4: Verify Docker Compose Installation
sudo docker-compose –version

https://bytexd.com/how-to-install-docker-compose-on-rhel-8-almalinux-rocky-linux/


### clone this repo
https://github.com/mdnahidmondol/Nitrate.git

cd Nitrate

### Run docker-compose File

sudo docker-compose up -d

### Stop docker-compose 

sudo docker-compose down