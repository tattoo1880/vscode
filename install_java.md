```shell
wget https://download.oracle.com/java/21/archive/jdk-21.0.7_linux-x64_bin.tar.gz


# 最新下载
wget https://download.oracle.com/java/21/latest/jdk-21_linux-x64_bin.tar.gz
sudo tar -C /usr/local -xzf jdk-21_linux-x64_bin.tar.gz 
# 找到实际安装路径
nano ~/.zshrc
export JAVA_HOME=/usr/local/jdk-21.0.10 
export PATH=$PATH:$JAVA_HOME/bin
source ~/.zshrc
```
