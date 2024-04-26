Alpine seems to be drastically smaller in size: 
```shell
>docker image ls | FINDSTR "devopsdockeruh"
devopsdockeruh/simple-web-service   ubuntu            4e3362e907d5   3 years ago   83MB
devopsdockeruh/simple-web-service   alpine            fd312adc88e0   3 years ago   15.7MB
```

```shell
>docker run -d --name alpine devopsdockeruh/simple-web-service:alpine
da774e39a52977ba0943c491c7ff50f3186fd3ffa51cc4736af70c0a1fcab8ae

>docker exec -it alpine sh
/usr/src/app # tail -f ./text.log
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-26 18:16:28 +0000 UTC
2024-04-26 18:16:30 +0000 UTC
2024-04-26 18:16:32 +0000 UTC
2024-04-26 18:16:34 +0000 UTC
2024-04-26 18:16:36 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-26 18:16:38 +0000 UTC
2024-04-26 18:16:40 +0000 UTC
2024-04-26 18:16:42 +0000 UTC
2024-04-26 18:16:44 +0000 UTC
2024-04-26 18:16:46 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-26 18:16:48 +0000 UTC
^C
/usr/src/app # exit

What's next?
  Try Docker Debug for seamless, persistent debugging tools in any container or image → docker debug alpine
  Learn more at https://docs.docker.com/go/debug-cli/
```
