# aitree — 個人投資 Dashboard

自動部署到 https://aitree.08creative.cc  （Cloudflare Pages）

## 來源

由 `~/ai-quant-workspace/generate_my_dashboard.py` 每日 3 次生成，
內容包含：
- Sinotrade 帳戶總覽
- 目前持股 + AI 建議
- 今日行動提示
- Watchlist Committee 排名
- 即時報價

## 部署

`~/ai-quant-workspace/deploy_dashboard.sh` 會：
1. Copy `my_dashboard.html` → `index.html`
2. `git add . && git commit && git push`
3. Cloudflare Pages 監控 → 自動部署

## 更新頻率

週一至週五 10:05 / 12:05 / 13:25（cron）
