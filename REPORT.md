# Báo cáo: Kiểm tra cài đặt Docker Engine & Chạy Hello-World

## 1. Kết quả lệnh docker version
```text
Client: Docker Engine - Community
 Version:           26.1.0
 API version:       1.45
 Go version:        go1.21.9
 Git commit:        9714adc
 Built:             Mon Apr 22 17:05:32 2024
 OS/Arch:           linux/amd64
 Context:           default

Server: Docker Engine - Community
 Engine:
  Version:          26.1.0
  API version:      1.45 (minimum version 1.24)
  Go version:       go1.21.9
  Git commit:       c8af8fe
  Built:            Mon Apr 22 17:05:32 2024
  OS/Arch:          linux/amd64
  Experimental:     false
 containerd:
  Version:          1.6.31
 runc:
  Version:          1.1.12
 docker-init:
  Version:          0.19.0

```

## 2. Kết quả lệnh docker info

```text
Client: Docker Engine - Community
 Version:    26.1.0
 Context:    default
 Debug Mode: false

Server:
 Containers: 1
  Running: 0
  Paused: 0
  Stopped: 1
 Images: 1
 Server Version: 26.1.0
 Storage Driver: overlay2
  Backing Filesystem: extfs
 Logging Driver: json-file
 Cgroup Driver: systemd
 Cgroup Version: 2
 Operating System: Ubuntu 22.04.4 LTS
 OSType: linux
 Architecture: x86_64
 CPUs: 4
 Total Memory: 7.688GiB
 Name: dev-workstation
 Docker Root Dir: /var/lib/docker

```

## 3. Kết quả lệnh docker run hello-world

```text
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
2db297d0c72f: Pull complete 
Digest: sha256:4bd78c129f2594da05e4e54500604981845032ab3044411602377823237b01c8
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

```