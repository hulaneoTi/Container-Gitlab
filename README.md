# Container-Gitlab

Senha inicial do root:
Password inicial do GITLAB:
    sudo docker exec -it gitlab grep 'Password:' /etc/gitlab/initial_root_password
Caso dê erro ao carregar o SONARQUBE:
    sudo sysctl -w vm.max_map_count=262144
Caso dê erro de permissão no Sonarqube:
    myname=$( [ "$(whoami)" = "root" ] && echo "$SUDO_USER" || whoami )
    sudo chown -R 1000:1000 /home/${myname}/gitlab/sonarqube/sonarqube_data
    sudo chown -R 1000:1000 /home/${myname}/gitlab/sonarqube/sonarqube_extensions
    sudo chown -R 1000:1000 /home/${myname}/gitlab/sonarqube/sonarqube_logs

