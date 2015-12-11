# **<center>還原 本機</center>**

---

#### 1. 使用putty登入伺服器(已完成請往下一步)
![](../img/inst_part1/part1_4.png)

#### 2. 將還原程序放入/var/www/html/data/中
### ```sudo mv utility/restore.php /var/www/html/data/```
![](../img/sr_part1/part1_1.png)

#### 3. 從本機chrome登入管理者admin帳號右上角進入【管理中心】
![](../img/bkup_part1/part1_1.png)

#### 4. 上排分類中選擇【站長】
![](../img/bkup_part1/part1_2.png)

#### 5. 左排功能中選擇【數據庫】
![](../img/bkup_part1/part1_3.png)

#### 6. 選擇數據庫頁面上排的【恢復】，指定以前備份過的後台設定，按導入
![](../img/sr_part1/part1_2.png)

#### 7. 等待導入ing…
![](../img/sr_part1/part1_3.png)

#### 8. 完成導入
![](../img/sr_part1/part1_4.png)

#### 9. 刪除還原程序
### ```sudo rm -rf /var/www/html/data/restore.php```
![](../img/sr_part1/part1_5.png)