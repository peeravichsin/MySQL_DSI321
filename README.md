# On implement Project

## Setup & Installtion

clone code to your working directory
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

To setup your Linux VMs in Azure 
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

1. For create a MySQL svever
```bash
docker-compose up --build
```
2. Then press CTRL+C when process done

3. And then compose up again and you are good to go :)
```bash
docker-compose up
```



