# 股票資訊查詢系統

這個 Flask 應用程式能夠幫助使用者查詢和顯示股票資訊，當使用者透過前端的表單頁面輸入資料，系統將從 Yahoo Finance 及時爬取股票，並將這些資料存儲到本地的 SQLite 資料庫中。  
用戶可以從前端頁面查看票的詳細資訊，包括成交量、最終價、開盤價、最高價、最低價、昨日收盤價、漲跌、漲跌幅和最後更新時間。  
 
#Requirements

 Python 3.x
 Flask
 SQLAlchemy
 Selenium
 BeautifulSoup
 Chrome 瀏覽器及其 WebDriver
