# 🇨🇿 捷克 8 天情侶行程規劃表

互動式單頁 HTML 旅遊行程，規劃布拉格、波希米亞瑞士國家公園與庫倫洛夫（CK 小鎮）的 8 天情侶旅遊。無需伺服器，開啟 HTML 檔案即可使用。

---

## ✨ 功能總覽

| 分頁 | 功能 |
|---|---|
| 📅 行程表 | 8 天行程展開卡片，右側嵌入地圖，含景點路線連線 |
| ✅ 出發清單 | 可新增、編輯、勾選、拖曳排序，完成項目自動移至最下方，顯示總費用統計 |
| 📋 預約管理 | 6 項預設預約景點，可拖曳排序、上傳確認截圖、輸入訂位代碼，可自行新增 |
| 📱 推薦 APP | 10 個旅遊必備 APP 說明清單 |

---

## 🗺 行程概覽

```
Day 1   台灣出發 → 布拉格抵達・河岸散步調時差
Day 2   布拉格老城區・天文鐘・查理大學・查理大橋・Vinohrady 咖啡區
Day 3   城堡區・Strahov 修道院圖書館・Beer Spa 啤酒溫泉・遊船晚餐
Day 4   波希米亞瑞士國家公園・砂岩石拱・峽谷船遊（可選跨境德國）
Day 5   布拉格 → Hluboká 城堡（順路停）→ CK 小鎮抵達
Day 6   CK 小鎮全天・古裝拍照・泛舟・啤酒廠・河岸晚餐
Day 7   CK → (Holašovice 可選) → 布拉格・購物・U Fleků 晚餐
Day 8   回台灣
```

### 住宿

| 城市 | 住宿 | 日期 |
|---|---|---|
| 布拉格 | NOBILIS RESIDENCE（備註 4 樓以上） | 8/1–8/5 |
| CK 小鎮 | Hotel Dvorak Český Krumlov | 8/5–8/7 |

---

## 📁 檔案結構

```
.
└── czech_itinerary.html   # 單一 HTML 檔案，含所有 CSS、JS、Leaflet 地圖
```

所有資源均內嵌於單一 `.html` 檔案中，無外部依賴（地圖底圖除外，需網路連線載入 OpenStreetMap 圖磚）。

---

## 🚀 使用方式

### 本地開啟

直接用瀏覽器開啟 HTML 檔案即可，無需安裝任何套件或伺服器：

```bash
# 下載後直接雙擊，或：
open czech_itinerary.html        # macOS
start czech_itinerary.html       # Windows
xdg-open czech_itinerary.html   # Linux
```

### GitHub Pages 部署

1. Fork 或上傳此 repo
2. 進入 **Settings → Pages**
3. Source 選擇 `main` branch，根目錄 `/`
4. 儲存後取得公開連結，即可在任何裝置瀏覽

---

## 🛠 技術細節

| 項目 | 說明 |
|---|---|
| 語言 | 純 HTML / CSS / Vanilla JavaScript |
| 地圖 | [Leaflet.js](https://leafletjs.com/) v1.9.4（內嵌，無 CDN 依賴） |
| 地圖底圖 | [OpenStreetMap](https://www.openstreetmap.org/)（需網路） |
| 字型 | Google Fonts：Cormorant Garamond、DM Sans |
| 資料儲存 | `localStorage`（清單、預約記錄存於瀏覽器本地） |
| 框架 | 無，純原生 JS |

### 地圖懶載入機制

所有地圖採用**懶載入**策略：每個行程天的地圖僅在使用者點開該天卡片時才初始化，避免頁面載入時容器高度為 0 導致地圖空白的問題。

---

## 📋 預設預約項目

| 景點 | 地點 | 建議時間 |
|---|---|---|
| 🍺 Beer Spa Bernard | 布拉格・Majestic Plaza 飯店 | Day 3 下午 |
| 📸 Seidel 攝影博物館古裝拍照 | CK 小鎮 | Day 6 上午（建議提前 1 個月預約） |
| ⛵ 遊船晚餐 | 布拉格・伏爾塔瓦河 | Day 3 晚上 |
| 🪨 波希米亞瑞士一日遊 | 布拉格出發 | Day 4 全天 |
| 🏰 布拉格城堡 B 票 | 布拉格・城堡區 | Day 3 上午 |
| 🎓 查理大學 Carolinum | 布拉格・老城區 | Day 2（免費） |

---

## 💾 資料說明

出發清單與預約記錄儲存於**瀏覽器 `localStorage`**，關閉分頁後資料仍會保留。清除瀏覽器快取或使用無痕模式會導致資料遺失，建議定期截圖備份重要訂位資訊。

---

## 📱 支援裝置

| 裝置 | 支援狀況 |
|---|---|
| 桌機瀏覽器 | ✅ 完整支援 |
| 平板 | ✅ 完整支援 |
| 手機 | ✅ 響應式設計，窄版自動調整 |

建議使用 Chrome、Safari、Firefox 等現代瀏覽器，IE 不支援。

---

## 🙏 資料來源

- 景點資訊：Google Maps、各官方網站
- 地圖：© [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors
- 住宿評價：Booking.com、Tripadvisor

---

*最後更新：2026 年 8 月出發版本*
