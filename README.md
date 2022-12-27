# Travel-Recommendation-System
## 彙整美國各城市熱門討論景點資訊 <br>


#### 方法：<br>

- 後端——網路爬蟲<br>
程式碼檔案為：``spider_google_and_reddit.ipynb``<br>

以網路爬蟲，爬取以下兩個網站資訊：<br>
1. Google Map: 以城市作為中心爬下在Google Map 有列出的景點、景點評分星級、景點基本資訊。<br>
2. Reddit: 以上述爬完的景點為list，在Reddit 旅遊版搜尋景點名稱，爬下有提到此景點的發文數、所有文章的留言數加總、所有文章的按讚數加總。<br>

以上資料存在MongoDB 資料庫中，分別為「TravelSite」和「SiteTrend」。


- 前端——Tableau 儀表板呈現<br>

  - 從MongoDB 資料庫撈取資料，程式碼：``ConnectDB.ipynb``<br>，輸出為[data](https://github.com/teng-yu-an/Travel-Recommendation-System/tree/main/data)資料夾內的``Travel.xlsx``。<br>
  - Tableau 儀表板檔案為：``w2g_ver3.twb``，並連結[data](https://github.com/teng-yu-an/Travel-Recommendation-System/tree/main/data)資料夾內的``data_for_Tableau.csv``資料。
