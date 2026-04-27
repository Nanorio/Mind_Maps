# 远程拉取
<hr />

### 容器运行
docker run -it --rm \
--name labelImg \
-e DISPLAY=$DISPLAY  \
-v /tmp/.X11-unix:/tmp/.X11-unix  \
-v $HOME:/app/data  \
labelimg:ubuntu20_x64 &







# 自行编译