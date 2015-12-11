# **<center>還原 移植</center>**

---

#### 1. 使用putty登入伺服器（已完成請往下一步）
![](../img/inst_part1/part1_4.png)

#### 2. 切換到專門放會員頭像的前一個目錄
### ```cd /var/www/html/uc_server/data/```

#### 3. 確定一次data目錄底下是否有avatar這個目錄
### ```ls```

#### 4. 修改avatar目錄名稱（不建議直接砍掉目錄，留著失敗了還能還原）
### ```sudo mv avatar avatar~```

#### 5. 確定avatar目錄名稱是否修改為avatar~了
### ```ls```

#### 6. 切換到bkup目錄
### ```cd ../../bkup```