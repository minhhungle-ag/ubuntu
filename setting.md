## IBus-Bamboo
sudo add-apt-repository ppa:bamboo-engine/ibus-bamboo
sudo apt-get update
sudo apt-get install ibus-bamboo
ibus restart

## Nvidia Installation
ubuntu-drivers devices
sudo ubuntu-drivers autoinstall
sudo apt install nvidia-driver-390
sudo reboot

## Git
sudo apt install git

## setup git 
ssh-keygen -t rsa -b 4096 -C "your_email@example.com" 
ssh-keygen -t ed25519 -C "your_email@example.com"


eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa

cat ~/.ssh/id_rsa.pub
ssh -T git@github.com

## ssh file
    # working account
        Host github.com
        HostName github.com
        User git
        IdentityFile ~/.ssh/id_rsa_work

    # personal account
        Host github.com-me
        HostName github.com
        User git
        IdentityFile ~/.ssh/id_rsa

    # personal account 
        Host github.com
        HostName github.com 
        User git 
        IdentityFile ~/.ssh/id_rsa
    
    # Private GitLab instance
        Host git@gitlab.company.com
        PreferredAuthentications publickey
        IdentityFile ~/.ssh/id_ed25519

## node
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash

nvm install 18.15.0
npm install -g yarn
    
## ts-node
npm install -g typescript ts-node tslib @types/node

## Postman
sudo snap install postman

## figma
sudo snap install figma-linux

## fira code
sudo add-apt-repository universe
sudo apt install fonts-firacode