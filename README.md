# SPY Intraday Chart（公開版）

SPY（S&P 500 ETF）1 分鐘 K 線走勢圖。**只顯示股價，不含任何交易紀錄。**

- 網頁：https://shuye1668.github.io/spy-intraday-chart/
- 資料由 GitHub Actions 每日以 yfinance 自動更新（美股盤中每 30 分、收盤定版）。
- **完全在雲端運作，與任何本機主機無關** —— 主機關機也持續更新。

## 檔案
- `index.html` — 由 `trade_review_app.py` 前端建置成的靜態純 K 線版
- `data/YYYY-MM-DD.json` — 每日 candles（無 trades）
- `dates.json` / `meta.json` — 索引與最後更新時戳
- `export_candles.py` — Actions 用來抓 yfinance 更新
- `.github/workflows/update.yml` — 排程

免責：僅供研究參考，不構成投資建議；資料可能延遲或有誤。
