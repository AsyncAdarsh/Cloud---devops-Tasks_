- name: Install Nginx on Devops-workstaion server
  host: all
  become: yes 
  

  tasks:
    -name: Install nginx
     yum:
       name: nginx 
       state: present 


    Docker
#Docker installation & first Container
docker --version
docker run ubuntu echo "Hello Workstation"

#Docker file
FROM ubuntu:22.04
CMD ["echo","Hello Workstation"]

