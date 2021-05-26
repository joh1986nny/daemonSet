# daemonSet

## 1. RSYSLOG
### 1.1 Descarga contenedor Docker
> docker pull rsyslog/syslog_appliance_alpine
```
johnny@johnny-inetum:~/daemonSet$ docker pull rsyslog/syslog_appliance_alpine
Using default tag: latest
latest: Pulling from rsyslog/syslog_appliance_alpine
2fdfe1cd78c2: Pull complete 
51631cad5a67: Pull complete 
bc03ff7bc61a: Pull complete 
c7ad936bdd12: Pull complete 
0f9163febd6d: Pull complete 
76f98260bbb2: Pull complete 
0164f652db31: Pull complete 
9b830923a0f2: Pull complete 
d9bc51ea5e92: Pull complete 
dc9573124a00: Pull complete 
933f52ce59f4: Pull complete 
Digest: sha256:c0dd7cad9ff3234967ff59879590175b7590e8a5f5621ec49a85aff546b44a3b
Status: Downloaded newer image for rsyslog/syslog_appliance_alpine:latest
docker.io/rsyslog/syslog_appliance_alpine:latest
```
### 1.2 Correr contenedor con rsyslog
> docker run rsyslog/syslog_appliance_alpine
```
johnny@johnny-inetum:~/daemonSet$ docker run -d rsyslog/syslog_appliance_alpine
dbc8fddccb650312272007c5627f0830df4c53a95a73d6f50358a53ef4e8f40c
```

### 1.3 Comprobar contenedores activos
> docker ps
```
johnny@johnny-inetum:~/daemonSet$ docker ps
CONTAINER ID   IMAGE                             COMMAND                  CREATED         STATUS         PORTS     NAMES
dbc8fddccb65   rsyslog/syslog_appliance_alpine   "/home/appliance/sta…"   7 seconds ago   Up 7 seconds             sweet_keldysh
```