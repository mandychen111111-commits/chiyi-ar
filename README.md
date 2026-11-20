# chiyi-ar — 掃碼 AR 產品頁

- 首頁：AR 檢視器（選擇模擬器下載的 .zip 即可進 AR）
- 產品頁：`/p/<slug>`，資料在 `products.json`，模型放在 `models/<slug>.glb` / `.usdz`

## 新增產品
1. 從包裝 AR 模擬器下載 AR 檔（.zip），解壓得到 .glb 與 .usdz
2. 改名為 `<slug>.glb`、`<slug>.usdz` 放進 `models/`
3. 在 `products.json` 加一筆：`"<slug>": {"title": "產品名", "desc": "說明", "model": "/models/<slug>"}`
4. 推上 GitHub，Vercel 自動更新；產品網址為 `https://chiyi-ar.vercel.app/p/<slug>`
