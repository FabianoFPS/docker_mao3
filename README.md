# docker_mao3
Exemplo de utilização do Docker - Docker hub - (local?)
https://docs.docker.com/install/linux/linux-postinstall/
https://gist.github.com/gabrielfroes/64193efbaf6dd2728e3a6dd4a1845941

Após instalação Docker:
Create the docker group.

$ sudo groupadd docker
Add your user to the docker group.

$ sudo usermod -aG docker $USER

*deslogar

$ systemctl stop docker
$ sudo nohup docker daemon -H tcp://0.0.0.0:2375 -H unix:///var/run/docker.sock &
$ systemctl start docker
$ sudo docker info
