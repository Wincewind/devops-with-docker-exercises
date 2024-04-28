```shell
>docker run -p 127.0.0.1:3000:8080 web-server
[GIN-debug] [WARNING] Creating an Engine instance with the Logger and Recovery middleware already attached.

[GIN-debug] [WARNING] Running in "debug" mode. Switch to "release" mode in production.
 - using env:   export GIN_MODE=release
 - using code:  gin.SetMode(gin.ReleaseMode)

[GIN-debug] GET    /*path                    --> server.Start.func1 (3 handlers)
[GIN-debug] Listening and serving HTTP on :8080
[GIN] 2024/04/28 - 08:27:49 | 200 |      27.101µs |      172.17.0.1 | GET      "/"
[GIN] 2024/04/28 - 08:27:49 | 200 |        13.9µs |      172.17.0.1 | GET      "/favicon.ico"
```