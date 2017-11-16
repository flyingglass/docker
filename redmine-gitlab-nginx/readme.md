### docker config redmine gitlab jenkins and use nginx proxy
1. mkdir -p /srv/docker/jenkins/jenkins
2. chown 1000 /srv/docker/jenkins/jenkins or chmod 777 /srv/docker/jenkins/jenkins
3. check docker-compose.yml proxy port, the default is 80
4. done!!!

redmine: https://github.com/sameersbn/docker-redmine
gitlab: https://github.com/sameersbn/docker-gitlab
