# install docker/docker-compose 

## install docker 

```
ssh -i /path/private_key.pem ec2-user@xx.xx.xx.xx

sudo yum update -y  
sudo yum install -y docker
sudo usermod -a -G docker ec2-user

sudo systemctl enable docker
sudo systemctl start docker
```

> https://docs.aws.amazon.com/ja_jp/AmazonECS/latest/developerguide/docker-basics.html


## install docker-compose 
```
sudo curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m) -o /usr/bin/docker-compose

sudo chmod +x /usr/bin/docker-compose
```

> https://docs.docker.com/compose/install/


