```shell
mkdir /etc/hysteria

openssl req -x509 -nodes -newkey ec:<(openssl ecparam -name prime256v1) -keyout /etc/hysteria/server.key -out /etc/hysteria/server.crt -subj "/CN=bing.com" -days 36500
sudo chmod +x /etc/hysteria

wget https://download.hysteria.network/app/latest/hysteria-linux-amd64-avx

cd /home/hys
nano config.yaml

listen: :443 #监听端口

tls:
  cert: /etc/hysteria/server.crt
  key: /etc/hysteria/server.key

auth:
  type: password
  password: 7788421

masquerade:
  type: proxy
  proxy:
    url: https://bing.com/
    rewriteHost: true

./hy server
