Secret message is: 'You can find the source code here: https://github.com/docker-hy'

```shell
>docker run -d devopsdockeruh/simple-web-service:ubuntu
e575df2714386cf53ed3a969f0258cf448ef5f10919d53f7c320b9f2270ba00c

>docker ps
CONTAINER ID   IMAGE                                      COMMAND                 CREATED          STATUS          PORTS     NAMES
e575df271438   devopsdockeruh/simple-web-service:ubuntu   "/usr/src/app/server"   19 seconds ago   Up 18 seconds             funny_almeida

>docker exec -it funny_almeida bash
root@e575df271438:/usr/src/app# tail -f ./text.log
2024-04-26 14:27:50 +0000 UTC
2024-04-26 14:27:52 +0000 UTC
2024-04-26 14:27:54 +0000 UTC
2024-04-26 14:27:56 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-26 14:27:58 +0000 UTC
2024-04-26 14:28:00 +0000 UTC
2024-04-26 14:28:02 +0000 UTC
2024-04-26 14:28:04 +0000 UTC
2024-04-26 14:28:06 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-26 14:28:08 +0000 UTC
2024-04-26 14:28:10 +0000 UTC
2024-04-26 14:28:12 +0000 UTC
^C
root@e575df271438:/usr/src/app# exit
exit

What's next?
  Try Docker Debug for seamless, persistent debugging tools in any container or image → docker debug funny_almeida
  Learn more at https://docs.docker.com/go/debug-cli/

```
