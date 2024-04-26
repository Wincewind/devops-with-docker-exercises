Before:
```shell
>docker ps -a
CONTAINER ID   IMAGE     COMMAND                  CREATED         STATUS                     PORTS     NAMES
2043a2f25594   nginx     "/docker-entrypoint.…"   8 minutes ago   Exited (0) 7 minutes ago             hopeful_boyd
debe1ab60146   nginx     "/docker-entrypoint.…"   8 minutes ago   Exited (0) 7 minutes ago             flamboyant_bardeen
9df0138aedb1   nginx     "/docker-entrypoint.…"   8 minutes ago   Up 8 minutes               80/tcp    stupefied_sammet

>docker image ls
REPOSITORY   TAG       IMAGE ID       CREATED      SIZE
nginx        latest    7383c266ef25   2 days ago   188MB
```
After:
```shell
>docker ps -a
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES

>docker image ls
REPOSITORY   TAG       IMAGE ID   CREATED   SIZE
```
