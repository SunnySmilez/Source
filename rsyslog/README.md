# 安装rsyslog
###### 由于本地下载rsyslog的源的速度太慢，每次timeout，因此，把下载好的rpm包直接存档，用本地安装解决
#### 安装rsyslog依赖包   
    yum localinstall libfastjson4-0.99.4-1.el6.x86_64.rpm 
    yum localinstall libgt-0.3.11-1.el6.x86_64.rpm

#### 安装rsyslog
    yum localinstall rsyslog-8.23.0-1.el6.x86_64.rpm

#### 检验是否安装成功
    rsyslogd -v

#### 启动
    /etc/init.d/rsyslog start
    ps aux | grep rsyslogd
    
#### 配置文件所在位置
    /etc/rsyslog.conf

##### 想搭建日志收集系统，查看更多rsyslog应用，请跳转：[rsyslog搭建日志系统](http://www.cxyteam.com/2016/12/19/rsyslog%E6%90%AD%E5%BB%BA%E6%97%A5%E5%BF%97%E7%B3%BB%E7%BB%9F/ "rsyslog搭建日志系统")
