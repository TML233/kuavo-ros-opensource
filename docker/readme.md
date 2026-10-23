## 容器使用说明
本机需要有x11桌面环境，容器内启动的窗口会在宿主机显示。

构建镜像：`make build` 或 `make buildx`
开启窗口穿透权限（宿主机重启后需要执行）：`make xhostallow`
启动容器：`make up`
关闭容器（内容将会消失）：`make down`
重启容器（内容不会消失）：`make restart`