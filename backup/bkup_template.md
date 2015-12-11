# **<center>備份 論壇模版**

---

#### 1. 使用putty登入伺服器（已完成請往下一步）
![](../img/inst_part1/part1_4.png)

#### 2. 安裝zip（已完成請往下一步）
### ```sudo apt-get install zip```
![](../img/bkup_part2/part2_1.png)

#### 3. 在伺服器目錄建立一個備份用的資料夾管理備份（已完成請往下一步）
### ```sudo mkdir /var/www/html/bkup```
![](../img/bkup_part2/part2_2.png)

#### 4. 切換到專門放論壇樣版的前一個目錄
### ```cd /var/www/html/```
![](../img/bkup_part4/part4_1.png)

#### 5. 接著把專門放論壇樣版的目錄壓縮成zip放進bkup資料夾
#### （記得用日期命名來管理備份內容，論壇愈大壓縮時間越長）
### ```sudo zip -r bkup/template151211.zip template/*```
![](../img/bkup_part4/part4_2.png)

#### 6. 需要還原請從【還原 附件檔案】參考還原的方式

#### ※論壇模版通常不會一直改變，不需要和其他備份一樣頻繁。

### **<center>以上就是在Linux中備份Discuz的教學！**
### **<center>Thanks for watching！**