# **<center>安裝 Discuz</center>**

---

#### 1. 下載Discuz安裝包
### ```wget 'http://download.comsenz.com/DiscuzX/3.1/Discuz_X3.1_TC_UTF8.zip'```
![](../img/inst_part3/part3_1.png)

#### 2. 查詢目前目錄底下是否有Discuz的壓縮檔
### ```ls```
![](../img/inst_part3/part3_2.png)

#### 3. 安裝unzip（為了對zip壓縮檔解壓縮）
### ```sudo apt-get install unzip```
![](../img/inst_part3/part3_3.png)

#### 4. 解壓縮Discuz_X3.1_TC_UTF8.zip
### ```sudo unzip Discuz_X3.1_TC_UTF8.zip```

#### 5. 再次查詢目前目錄底下應該多三個資料夾（readme、upload、utility）
#### （可以在自己本機端也下載一個Discuz_X3.1_TC_UTF8.zip比對內容比較清楚）
### ```ls```
![](../img/inst_part3/part3_4.png)

#### 6. 將upload資料夾內的所有檔案移動到伺服器的資料夾中
### ```sudo mv upload/* /var/www/html/```

#### 7. 回到本機chrome進入（虛擬機IP/install）就會看到Discuz安裝畫面（按我同意）
![](../img/inst_part3/part3_5.png)

#### 8. 接著如果看到目錄文件權限不足，就需要回到putty將資料夾的權限打開才能繼續安裝，沒有出現錯誤請從（12.）繼續往下
![](../img/inst_part3/part3_6.png)

#### 9. 先將目錄切換到伺服器的資料夾底下
### ```cd /var/www/html/```
![](../img/inst_part3/part3_7.png)

#### 10. 修改以下幾個目錄的權限（config、data、uc_server/data/、uc_client/data/cache）
### ```sudo chmod -R 777 config/ data/ uc_server/data/ uc_client/data/cache/```
![](../img/inst_part3/part3_8.png)

#### 11. 重新整理本機的chrome應該所有狀態都呈現打勾，就能拉到底部按下一步了
![](../img/inst_part3/part3_9.png)

#### 12. 選擇全新安裝 Discuz! X （含 UCenter Server）按下一步
![](../img/inst_part3/part3_10.png)

#### 13. 填寫數據庫信息的部分需要修改數據庫密碼（輸入MySQL的root密碼），填寫管理員信息的部分需要輸入管理員密碼（這是Discuz論壇的管理員密碼請記好）、重複密碼（管理員密碼），完成後按下一步
![](../img/inst_part3/part3_11.png)

#### 14. 等待安裝ing…
![](../img/inst_part3/part3_12.png)

#### 15. 安裝完成後點右下角有一行像是廣告的小字…(您的論壇已完成安裝，點此訪問)
![](../img/inst_part3/part3_13.png)

### 16. 這時chrome的網址應該是進入你的虛擬機ip，卻沒有進入論壇而是顯示apache的畫面
#### （如果不是顯示底下畫面請從(18.)繼續往下）
![](../img/inst_part1/part1_8.png)

#### 17. 因為預設第一順位是讓apache指定到index.html所以我們要修改他讓apache可以指定到論壇的頁面
### ```sudo mv /var/www/html/index.html /var/www/html/index~.html```
![](../img/inst_part3/part3_14.png)

#### 18. 回到本機chrome進入(虛擬機IP)
#### （如果出現下圖代表Discuz論壇已經安裝成功了！）
![](../img/inst_part3/part3_15.png)

#### 19. 安裝成功後要回到putty將安裝的程序刪除掉，否則其他人進入後也可以把你的論壇重新安裝！
### ```sudo rm /var/www/html/install/index.php```
![](../img/inst_part3/part3_16.png)

#### 20. 最後登入管理者做最後的確認，帳號：admin、密碼：(13.輸入的管理者密碼)
![](../img/inst_part3/part3_17.png)

### **<center>以上就是在Linux中安裝Discuz的教學！</center>**
### **<center>Thanks for watching！</center>**