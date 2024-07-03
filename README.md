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

## 使用教學  
輸入股票代碼： 在首頁的表單中，輸入1~5隻股票的代碼並提交。  
查看股票資訊： 提交後，將顯示股票代碼、公司名稱、成交量、最終價、開盤價、最高價、最低價、昨日收盤價、漲跌、漲跌幅和更新時間等詳細資訊。


