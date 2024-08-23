# How to Deploy a Wordpress and MySQL container application on Linux using Docker Compose

Pre-req

1. Ubuntu machine with ARM based
2. Install docker and docker-compose
3. Invoke the snippet using below link and name it "docker-compose.yaml"
4. Run it

## 1. Launch EC2 instance with Ubuntu

Login to AWS console and spinup the ubuntu instance with ARM based

![image](https://github.com/user-attachments/assets/ee595bc0-e92e-4f0f-a0ef-fd515c3f309c)

## 2. Install docker and docker-compose

```
sudo apt update
sudo apt install -y apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt update
sudo apt install -y docker-ce
sudo systemctl status docker
sudo usermod -aG docker $USER
sudo curl -L "https://github.com/docker/compose/releases/download/v2.20.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
docker-compose --version
```

## 3. Create a Docker-Compose yaml





