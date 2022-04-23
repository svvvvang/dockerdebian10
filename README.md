# Installing docker on debian 10 via commandline
sudo apt update
sudo apt upgrade
sudo reboot
sudo apt install docker.io

# Docker command can only be run with admin privileges. 
# For secrity purpose, add user to docker group
sudo usermod -a -G docker $USER

# Enable Docker daemon at boot
sudo systemctl start docker
sudo systemctl enable docker

# Stop or restart Docker daemon 
sudo systemctl stop docker
sudo systemctl restart docker

# Images on local system
docker images

# Images search
docker search <name of image>
  
# Image pull
docker oull <name of image>



