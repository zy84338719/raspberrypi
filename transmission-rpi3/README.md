# Transmission Docker file for Raspberry Pi 3

docker run -i --restart=always --net=bridge -d \
--name=transmission \
--hostname=transmission \
-p 9091:9091 \
-p 51413:51413 \
-v /CONFIG__Fix:/root/.config/transmission-daemon \
-v /PT/downloads:/downloads \
-v /PT/volume/files:/files \
-v /PT/watchdir:/watchdir \
-v /PT/volume/incomplete:/incomplete \
transmission-rpi3:latest


请将配置文件复制到/root/.config/transmission-daemon \
