# 股票資訊查詢系統

## 概述

這個 Flask 應用程式能夠幫助使用者查詢和顯示股票資訊，當使用者透過前端的表單頁面輸入資料，系統將從 Yahoo Finance 及時爬取股票，並將這些資料存儲到本地的 SQLite 資料庫中。  
用戶可以從前端頁面查看票的詳細資訊，包括成交量、最終價、開盤價、最高價、最低價、昨日收盤價、漲跌、漲跌幅和最後更新時間。  

## Requirements 

在開始使用之前，請確保你的開發環境中安裝了以下模組或插件：

- Python 3.x
- Flask
- SQLAlchemy
- Selenium
- BeautifulSoup
- Chrome 瀏覽器及其 WebDriver

## 安裝與設置

1. 下載程式碼  
git clone <repository-url>
cd stock-data-web-app  

3. 安裝套件  
pip install -r requirements.txt  

4. 執行程式  
python app.py  

5. 開啟瀏覽器  
在瀏覽器中輸入 http://127.0.0.1:5000/ 以訪問應用程式。

## 使用教學與流程  

輸入股票代碼：   
在首頁的表單中，輸入1~5隻股票的代碼並提交。  (範例為抓取2隻股票代碼)  
![Image text](https://github.com/viang2593/Daphne_stocks/blob/e98bb53cb773af00ebac610a7ef6759b07d76832/image/%E8%BC%B8%E5%85%A5%E8%82%A1%E7%A5%A8%E4%BB%A3%E7%A2%BC.png)  

獲取股票資訊：  
提交後，將顯示股票代碼、公司名稱、成交量、最終價、開盤價、最高價、最低價、昨日收盤價、漲跌、漲跌幅和更新時間等詳細資訊。  
![Image text](https://github.com/viang2593/Daphne_stocks/blob/4f1f063bc7226a7016ea0becbbd7159d3e0342a0/image/%E7%8D%B2%E5%BE%97%E8%82%A1%E7%A5%A8%E8%B3%87%E8%A8%8A.png)  

存進資料庫：  
資料抓取後會自動存入資料庫，若關閉後再開啟新頁面則資料庫會清空。  
![Image text](https://github.com/viang2593/Daphne_stocks/blob/4f1f063bc7226a7016ea0becbbd7159d3e0342a0/image/%E6%88%90%E5%8A%9F%E5%AD%98%E5%85%A5%E8%B3%87%E6%96%99%E5%BA%AB.png)  

### 最多一次可以抓取五支股票!
![Image text](https://github.com/viang2593/Daphne_stocks/blob/4f1f063bc7226a7016ea0becbbd7159d3e0342a0/image/%E6%9C%80%E5%A4%9A%E7%88%AC%E5%8F%965%E9%9A%BB.png)

在未關閉頁面的情況下也都會成功存入資料庫
![Image text](https://github.com/viang2593/Daphne_stocks/blob/d8e847b326b4e9f920253abd91ad983e21ea6afe/image/%E5%85%A8%E9%83%A8%E9%83%BD%E6%9C%89%E6%88%90%E5%8A%9F%E5%AD%98%E5%85%A5.png)

# 感謝您的觀看!
