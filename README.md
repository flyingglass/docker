# docker

- gitlab-redmine 目录 可供docker单独部署gitlab，redmine
- redmine-gitlab-nignx 目录 可供docker nginx容器代理gitlab, redmine, jenkins
- showdoc 目录 可供docker单独部署showdoc
- nexus首次启动会出现权限不足的问题, 赋予权限chown 200 -R /srv/docker/nexus/nexus-data
- 最外层docker-compose.yml 可供docker部署gitlab redmine showdoc nexus,宿主机部署jenkins,
并且采用nginx作为代理,其中jenkins部署启动需要附带--prefix=jenkins 否则nginx代理会失败

