# travellerDockerCompose
Repository, which consist docker compose file for running traveller

# Getting Started

### Reference Documentation

To run the project you have to install docker and docker-compose:
* sudo apt-get update
* sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
* curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
* echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
* sudo apt-get update
* sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin

* DOCKER_CONFIG=${DOCKER_CONFIG:-$HOME/.docker}
* mkdir -p $DOCKER_CONFIG/cli-plugins
* curl -SL https://github.com/docker/compose/releases/download/v2.4.1/docker-compose-linux-x86_64 -o $DOCKER_CONFIG/cli-plugins/docker-compose
* chmod +x $DOCKER_CONFIG/cli-plugins/docker-compose

### Guides

Run application:
* docker-compose up --build