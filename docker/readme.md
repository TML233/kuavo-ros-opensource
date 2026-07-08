## 容器使用说明

#### 1. 构建容器镜像
- 根据Dockerfile文件构建容器镜像，运行以下命令：

```bash
./build_image.sh
```

#### 2. 运行容器
- 运行容器需要配置一些环境变量，挂载目录等，所以提供了一些运行脚本方便使用。
- 普通运行(cpu)，没有GPU或者没有配置好`nvidia-container-toolkit`的机器，运行以下命令：
```bash
./run_with_cpu.sh
```

- 运行GPU版本，需要配置好`nvidia-container-toolkit`和`nvidia-runtime`等环境变量，可以在带GPU的宿主机上mujoco、gazebo等仿真更流畅
```bash
./run_with_gpu.sh
```

