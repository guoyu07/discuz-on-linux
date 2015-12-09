# **安裝lamp & phpmyadmin**


### 1. 確認網路狀態
## ```ping -c 3 www.google.com```
![](img/p1_1.png)

### 2. 安裝ssh
## ```sudo apt-get install ssh```
![](img/p1_2.png)

### 3. 透過ifconfig eth0或eth1取得虛擬機的IP

## ```ifconfig eth1```
![](img/p1_3.png)

### 4. 從本機開啟putty進入server，第一次會出現警告按ok即可
![](img/p1_4.png)

### 5. 登入後將VirtualBox的視窗縮小，用putty操作比較方便

![](img/p1_5.png)

### 6. 安裝lamp
## ```sudo tasksel install lampserver```