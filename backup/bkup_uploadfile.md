# **<center>備份 附件檔案</center>**

---

#### 1. 使用putty登入伺服器(已完成請往下一步)
![](../img/inst_part1/part1_4.png)

#### 2. 安裝zip
### ```sudo apt-get install zip```
![](../img/bkup_part2/part2_1.png)

#### 3. 在伺服器目錄建立一個備份用的資料夾管理備份
### ```sudo mkdir /var/www/html/bkup```
![](../img/bkup_part2/part2_2.png)

#### 4. 切換到專門放附件檔案的目錄
### ```cd /var/www/html/data/attachment/```
![](../img/bkup_part2/part3_1.png)

#### 5. 接著把專門附件檔案的目錄壓縮成zip放進bkup資料夾
#### （記得用日期命名來管理備份內容，論壇愈大壓縮時間越長）
### ```sudo zip -r ../../../bkup/attachment151211.zip /var/www/html/data/attachment/```
![](../img/bkup_part3/part3_2.png)