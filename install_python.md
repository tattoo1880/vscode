```shell
wget https://www.python.org/ftp/python/3.13.7/Python-3.13.7.tar.xz
sudo apt update
sudo apt install -y build-essential libssl-dev zlib1g-dev libncurses5-dev libncursesw5-dev libreadline-dev libsqlite3-dev libgdbm-dev libdb5.3-dev libbz2-dev libexpat1-dev liblzma-dev tk-dev libffi-dev
tar -xf Python-3.13.7.tar.xz
cd Python-3.12.4
./configure
make -j $(nproc)
sudo make altinstall
```


```shell
sudo update-alternatives --install /usr/bin/python3 python3 /usr/local/bin/python3.12 1
sudo update-alternatives --config python3
```
