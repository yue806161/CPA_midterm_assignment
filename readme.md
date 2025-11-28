# 中正 程式設計與應用 期中作業

環境名稱: ccu_CPA_midterm_homework

## 第一部分: 取得數據

  (25%) 抓取特斯拉、福特和通用汽車的股票價格（2013-2023 年）。

## 第二部分: 視覺化

  取得特斯拉、福特和通用汽車的股票價格 (2012 年)。
  並使用matplotlib, mplfinance視覺化

  1. (20%) 每家各別視覺化
  2. (5%) 三家合併到同一張圖中

## 第三部分: 基本財務分析

  1. (20%)為每個資料框建立一個名為 returns 的新欄位。該列的值將根據收盤價列計算得出。有兩種方法可以實現：一種是使用 .shift() 方法，並按照上述公式進行簡單計算；另一種是使用 pandas 內建的pct_change 方法。

  2. (5%) 繪製每家公司收益率的直方圖。可以分別繪製，也可以將它們疊在一起繪製。

## 第四部分: 每日累積收益率

  每日收益率 = (每日收盤價 - 昨日收盤價) / 昨日收盤價  
  累積收益率 = 目前價格  / 買入價格

  df[daily_cumulative_return] = ( 1 + df[pct_daily_return] ).cumprod()  
  ps: pct_daily_return 就是上一題的函式。

  1. (20%) Please Create a cumulative daily return column for each car company's dataframe, response the source code and results in your document.  
  2. (5%) Please plot three companies’ Cumulative Return columns against the time series index in one figure. And answer which stock showed the highest return for a $1 invested? Which showed the lowest?

## 學習目標

  1. 學習各 python 套件的使用。
  2. 如何執行該 Jupyter Notebook。
  3. 學習環境配置(mamba)。
