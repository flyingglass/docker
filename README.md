# docker

- gitlab-redmine 目录 可供docker单独部署gitlab，redmine
- redmine-gitlab-nigx 目录 可供docker nginx容器代理gitlab, redmine
- showdoc 目录 可供docker单独部署showdoc
- 最外层docker-compose.yml 目录可供docker部署gitlab redmine showdoc,宿主机部署jenkins，并且采用nginx作为代理
  jenkins部署启动需要附带--prefix=jenkins 否则nginx代理会失败
