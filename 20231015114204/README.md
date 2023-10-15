# Install docker and docker-compose script

```bash
curl -fsSL https://get.docker.com/ | sh
sudo systemctl enable --now docker
sudo usermod -aG docker $(whoami)
newgrp docker
sudo curl -L "https://github.com/docker/compose/releases/download/v2.20.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```

Tags:
```
#docker #docker-compose #install #linux #script
```

Related:
```
* Shahriar Nazemi
```
