# serj2t-kodekloud-k8s



Используемые команды
k create cm nginx-config --from-file=nginx.conf
k create cm nginx-config --from-file=nginx.conf
k cp /opt/index.php nginx-phpfpm:/usr/share/nginx -c nginx-container
k expose pod nginx-phpfpm --name=nginx-phpfpm-svc --type=NodePort
