```shell
wget https://download.oracle.com/java/21/archive/jdk-21.0.7_linux-x64_bin.tar.gz
sudo tar -C /usr/local -xzf jdk-21
# 找到实际安装路径
nano ~/.zshrc
export JAVA_HOME=/usr/local/jdk-21.0.7
export PATH=$PATH:$JAVA_HOME/bin
source ~/.zshrc
```
