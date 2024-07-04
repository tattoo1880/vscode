```shell
wget sudo tar -C /usr/local -xzf jdk-22_linux-x64_bin.tar.gz
sudo tar -C /usr/local -xzf jdk-22_linux-x64_bin.tar.gz
# 找到实际安装路径
nano ~/.zshrc
export JAVA_HOME=/usr/local/jdk-22
export PATH=$PATH:$JAVA_HOME/bin
source ~/.zshrc
```