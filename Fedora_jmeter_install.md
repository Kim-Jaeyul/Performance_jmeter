## 사전확인

- RHEL, CENTOS, FEDORA GUI로 설치

- Java 8이상

  ```
  [root@jmeter ~]# java -version
  openjdk version "1.8.0_262"
  OpenJDK Runtime Environment (build 1.8.0_262-b10)
  OpenJDK 64-Bit Server VM (build 25.262-b10, mixed mode)
  [root@jmeter ~]#
  ```

  

## 설치

```
[root@jmeter ~]# cd /usr/local/src/ 
[root@jmeter ~]# 
[root@jmeter ~]# export JMETER_VERSION=5.3
[root@jmeter ~]#
[root@jmeter ~]# wget -q https://archive.apache.org/dist/jmeter/binaries/apache-jmeter-$JMETER_VERSION.tgz
[root@jmeter ~]# ll
total 65796
-rw-------. 1 root root     2065 Nov 10 11:37 anaconda-ks.cfg
-rw-r--r--. 1 root root 67364344 Jul  3 13:29 apache-jmeter-5.3.tgz
drwxr-xr-x. 2 root root        6 Nov 10 11:48 Desktop
drwxr-xr-x. 2 root root        6 Nov 10 11:48 Documents
drwxr-xr-x. 2 root root        6 Nov 10 11:48 Downloads
-rw-r--r--. 1 root root     2158 Nov 10 11:38 initial-setup-ks.cfg
drwxr-xr-x. 2 root root        6 Nov 10 11:56 jmeter
drwxr-xr-x. 2 root root        6 Nov 10 11:48 Music
drwxr-xr-x. 2 root root        6 Nov 10 11:48 Pictures
drwxr-xr-x. 2 root root        6 Nov 10 11:48 Public
drwxr-xr-x. 2 root root        6 Nov 10 11:48 Templates
drwxr-xr-x. 2 root root        6 Nov 10 11:48 Videos
[root@jmeter ~]#
[root@jmeter ~]# tar -xzf apache-jmeter-$JMETER_VERSION.tgz 
[root@jmeter ~]# 
[root@jmeter ~]# mkdir -p /usr/local/jmeter
[root@jmeter ~]# 
[root@jmeter ~]# mv apache-jmeter-$JMETER_VERSION /usr/local/jmeter
[root@jmeter ~]# 
[root@jmeter ~]# export JMETER_HOME=/usr/local/jmeter/apache-jmeter-5.3
[root@jmeter ~]# 
[root@jmeter ~]# export PATH=$JMETER_HOME/bin:$PATH
[root@jmeter ~]# 
[root@jmeter ~]# jmeter -v
    _    ____   _    ____ _   _ _____       _ __  __ _____ _____ _____ ____
   / \  |  _ \ / \  / ___| | | | ____|     | |  \/  | ____|_   _| ____|  _ \
  / _ \ | |_) / _ \| |   | |_| |  _|    _  | | |\/| |  _|   | | |  _| | |_) |
 / ___ \|  __/ ___ \ |___|  _  | |___  | |_| | |  | | |___  | | | |___|  _ <
/_/   \_\_| /_/   \_\____|_| |_|_____|  \___/|_|  |_|_____| |_| |_____|_| \_\ 5.3

Copyright (c) 1999-2020 The Apache Software Foundation

[root@jmeter ~]#

```



## 실행

- GUI 터미널에서 실행

  ```
  [root@jmeter bin]# pwd
  /usr/local/jmeter/apache-jmeter-5.3/bin
  [root@jmeter bin]# ./jmeter
  ```

  

  











