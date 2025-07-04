<div align="center">

## **_mysql 的安装_**

---

![github star](https://img.shields.io/badge/tattoo1880-v_1.0-blue)

</div>


```shell
sudo apt update
sudo apt install mysql-server
```

### 让 mysql 可以被远程访问
```shell
sudo nano /etc/mysql/mysql.conf.d/mysqld.cnf
# 将 bind-ip 改成 0.0.0.0
sudo systemctl restart mysql
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'qwerty7788421';
FLUSH PRIVILEGES;
CREATE USER 'root'@'%' IDENTIFIED BY 'qwerty7788421';
GRANT ALL PRIVILEGES ON *.* TO 'root'@'%' WITH GRANT OPTION;
FLUSH PRIVILEGES;
```
