# 香港天文台 - 顯著降雨概率儀表元件 (SenseCraft HMI)

一個自包含 HTML 元件，用於 SenseCraft HMI。自動讀取天文台九天預報 API 的 PSR（顯著降雨概率），按程度顯示對應的天文台原裝雨傘圖示。

## 功能
- 5 個等級：低 (<30%) / 中低 (30-44%) / 中 (45-54%) / 中高 (55-69%) / 高 (≥70%)
- 5 張天文台原裝雨傘圖已內嵌於 HTML（Base64），無需另外載入圖片
- 每次刷新自動更新

## 在 SenseCraft HMI 使用
1. Canvas Designer → 數據 (Data) → HTML 組件
2. 貼上本 repo 的 GitHub Pages URL：`https://<你的用戶名>.github.io/hko-psr-dashboard/index.html`
3. 設定預覽尺寸 → Load → Confirm → Apply

## 檔案
- `index.html` — 主元件（圖片已內嵌）
- `images/` — 5 張天文台原裝雨傘圖 (PNG)
- `hko_icons.zip` — 天氣圖示包（如需其他天氣圖）

## 資料來源
- 香港天文台開放資料 API：`https://data.weather.gov.hk/weatherAPI/opendata/weather.php?dataType=fnd&lang=tc`
- 天氣圖示：https://www.hko.gov.hk/images/HKOWxIconOutline/pic*.png
- 降雨概率圖示：https://www.hko.gov.hk/common/images/PSR*_50_light.png