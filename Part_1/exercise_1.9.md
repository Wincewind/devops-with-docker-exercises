Exercise was done on Windows. After creating a file called `text.log` in the current directory:
```shell
>docker run -v "%cd%/text.log:/usr/src/app/text.log" devopsdockeruh/simple-web-service
```