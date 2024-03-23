## 其他

```
# 免密登录
ssh-keygen -t rsa -f ssh-key

vim authorized_keys
chmod 644 authorized_keys
```

```
# xfce4
echo xfce4-session > ~/.xsession
```

```
sudo adduser 
sudo usermod -G 
```


```
sudo vim  /etc/profile.d/proxy.sh
```

```
 # set proxy config via profie.d - should apply for all users
export http_proxy="http://10.201.34.195:7890/"
export https_proxy="http://10.201.34.195:7890/"
export ftp_proxy="http://10.201.34.195:7890/"
export no_proxy="127.0.0.1,localhost"
# For curl
export HTTP_PROXY="http://10.201.34.195:7890/"
export HTTPS_PROXY="http://10.201.34.195:7890/"
export FTP_PROXY="http://10.201.34.195:7890/"
export NO_PROXY="127.0.0.1,localhost"
#将要从代理中排除的其他IP添加到NO_PROXY和no_proxy环境变量中

```
```
sudo chmod +x  /etc/profile.d/proxy.sh
source /etc/profile.d/proxy.sh
#查看环境变量进行确认是否生效
env | grep -i proxy

```
