# DockAnsible
simulation of an Ansible environment using Docker Containers


![image](https://user-images.githubusercontent.com/108732943/203650459-fd84d8f4-153a-4b10-aef8-6055551539fc.png)





cd base
docker build -t ansible_base .


cd master/
docker build -t master .

cd host/
docker build -t host .



docker-compose up -d


