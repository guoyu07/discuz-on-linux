# **<center>安裝 phpmyadmin**

---

#### 1. 安裝phpmyadmin（需要…容量是否要安裝選 Y）
### ```sudo apt-get install phpmyadmin```
![](../img/inst_part2/part2_1.png)

#### 2. 選擇apache2→Ok
![](../img/inst_part2/part2_2.png)

#### 3. 選擇Yes
![](../img/inst_part2/part2_3.png)

#### 4. 輸入在【安裝 lamp-server（7.）MySQL的root密碼】
![](../img/inst_part2/part2_4.png)

#### 5. 再次輸入MySQL的root密碼
![](../img/inst_part2/part2_5.png)

#### 6. 最後再次輸入確認MySQL的root密碼
![](../img/inst_part2/part2_6.png)

#### 7. 安裝完成後，從本機開啟chrome進入（虛擬機IP/phpmyadmin），如果出現404Not Found，是因為apache沒有設定到，所以我們需要將phpmyadmin寫入apache的設定中，沒有出現下圖的畫面，請從（11.）繼續往下
![](../img/inst_part2/part2_7.png)

#### 8. 使用vim編輯器打開apache的設定檔
##```sudo vim /etc/apache2/apache2.conf```
![](../img/inst_part2/part2_8.png)

#### 9. 將要設定的phpmyadmin設定內容貼上（右鍵）並儲存（:wq）
###設定內容：```Include /etc/phpmyadmin/apache.conf```
###```進入編輯模式(I)→空行(Enter)→回上一行(↑)→貼上(右鍵)→離開編輯模式(Esc)→儲存並離開(:wq)→送出指令(Enter)```
![](../img/inst_part2/part2_9.png)

#### 10. 重新啟動apache（為了讓apache讀取剛剛修改的內容）
###```sudo service apache2 restart```
![](../img/inst_part2/part2_10.png)


#### 11. 再次從本機開啟chrome進入（虛擬機IP/phpmyadmin）
####（出現下圖代表phpmyadmin已安裝成功）
![](../img/inst_part2/part2_11.png)

###接著請跳下一章＞安裝 Discuz

