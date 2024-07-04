```shell
wget https://go.dev/dl/go1.22.5.linux-amd64.tar.gz
sudo tar -C /usr/local -xzf go1.22.5.linux-amd64.tar.gz
nano ~/.zshrc
export PATH=$PATH:/usr/local/go/bin
source ~/.zshrc
```