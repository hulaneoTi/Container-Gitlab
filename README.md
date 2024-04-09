# Container-Gitlab

Senha inicial do root:
Password inicial do GITLAB:
    sudo docker exec -it gitlab grep 'Password:' /etc/gitlab/initial_root_password
Caso dê erro ao carregar o SONARQUBE:
    sudo sysctl -w vm.max_map_count=262144
