# serj2t-kodekloud-k8s



### Используемые команды
```sh
k create cm nginx-config --from-file=nginx.conf
k apply -f 1.yaml
k expose pod nginx-phpfpm --name=nginx-phpfpm-svc --type=NodePort
k cp /opt/index.php nginx-phpfpm:/var/www/html -c nginx-container
```
