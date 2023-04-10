# code-server-docker

code server docker with dev env

## use

https://hub.docker.com/r/linuxserver/code-server

https://hub.docker.com/u/yongfeili

docker run -d \
 --name=code-server \
 -e PUID=1000 \
 -e PGID=1000 \
 -e TZ=Asia/Shanghai \
 -e PASSWORD=pwd `#optional` \
 -e HASHED_PASSWORD= `#optional` \
 -e SUDO_PASSWORD=pwd `#optional` \
 -e SUDO_PASSWORD_HASH= `#optional` \
 -e PROXY_DOMAIN=xx.xx.com `#optional` \
 -e DEFAULT_WORKSPACE=/config/workspace `#optional` \
 -p 8000:8443 \
 -v vs_code_server_config:/config \
 --restart unless-stopped \
 yongfeili/code-server-with-all-china:latest
