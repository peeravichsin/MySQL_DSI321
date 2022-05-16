# On implement Project

## Setup & Installtion

Clone code to your working directory
```bash
git clone https://github.com/peeravichsin/MySQL_DSI321
```

Install library for this Project

```bash
pip install -r requirements.txt
```

## Running The Website

Go to /web and then run this command below and website is running :)
```bash
python main.py
```


# Setup Docker in VM

## Setup & Installtion

1.Create Vms in Azure

2.Go to Networking and then Add inbound port rule follow this step below

 - source --> Any  
 - Source port ranges --> *
 - Destination --> Any
 - Service --> Custom
 - Destination port ranges --> 5000   (**Attention this is very important**)
 - Protocol --> Any
 - Action --> Allow
 - Priority --> Let Azure select for you Ex. 3xx 
 - Name --> "any name you like"
 - Description --> "any thing you want to describe"

3.Open Powershell and connect to Vms using ssh method
  
4.To setup your Linux VMs in Azure 
  
```bash
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install docker.io
sudo apt  install docker-compose
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker 
docker run hello-world
```

# Git Clone all the code to VMs

Clone code and resouce to VMs
```bash
git clone https://github.com/peeravichsin/MySQL_DSI321
```

# On deploy

In this step is a bit tricky here the solution

1. For create a MySQL svever and host the website 
```bash
docker-compose up --build
```

2. if you want to stop the process
```bash
docker-compose down
```

Thank you for reading :)

