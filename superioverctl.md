<div align="center">

## **supervisor 的安装_**

---

![github star](https://img.shields.io/badge/tattoo1880-v_1.0-blue)

</div>

### 安装supervisor
```shell
sudo apt-get update
sudo apt-get install supervisor
```

### 编写 conf
```shell
nano /etc/supervisor/conf.d/gomain.conf
```

```shell
[program:gomain]
command=/root/groqbot/main  
directory=/root/groqbot
autostart=true
autorestart=true
startsecs=10
user=root
redirect_stderr=true
stdout_logfile=/var/log/supervisor/hys.log
environment=HOME="/root",PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:"

```

```shell
sudo supervisorctl reread
sudo supervisorctl update
```