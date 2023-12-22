This is new repo to install odoo using docker


1) **Install docker 
**  
   = sudo apt-get update
  
  sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
  
  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
  
  sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
  
  sudo apt-get update
  
  sudo apt-get install docker-ce
  
  sudo systemctl status docker
  
  sudo usermod -aG docker ${USER} 
  
  sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
  
  
  sudo chmod +x /usr/local/bin/docker-compose
  docker-compose --version


2) Then clone this repo.

3) Your custom modules will be in extra-addons folder.

4) Your odoo.conf in config folder (If you want to change anything)

5) Run this command -> docker-compose up (You need to run this command in the folder where docker-compose.yml file exist.

6) Odoo will run on 8017 port : localhost:8017
