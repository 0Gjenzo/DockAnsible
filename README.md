# DockAnsible
simulation of an Ansible environment using Docker Containers

.
├── base
│   └── Dockerfile
├── docker-compose.yml
├── host
│   ├── Dockerfile
│   └── run.sh
├── master
│   ├── ansible
│   │   ├── install_php.yml
│   │   └── inventory
│   └── Dockerfile
├── portainer-data_2
│   ├── bin  [error opening dir]
│   ├── certs  [error opening dir]
│   ├── compose  [error opening dir]
│   ├── docker_config  [error opening dir]
│   ├── portainer.db
│   ├── portainer.key
│   ├── portainer.pub
│   └── tls  [error opening dir]
└── README.md

10 directories, 11 files




cd base
docker build -t ansible_base .


cd master/
docker build -t master .

cd host/
docker build -t host .



docker-compose up -d


