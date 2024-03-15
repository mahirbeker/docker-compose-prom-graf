install docker engine and docker-compose

You should add "docker" as a group, give permissions and restart docker.service
sudo gourpadd docker
sudo usermod -aG docker ${USER}
sudo chmod 666 /var/run/docker.sock 
sudo systemtl restart docker

You must change the volume paths and PUID-GUID number in the docker-compose.yml file before the docker-compose up command.
