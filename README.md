# GTC Taipei 2026 Keynote · 多受眾導覽地圖

把黃仁勳 GTC Taipei 2026 主題演講，切成 **13 個主題 × 4 種受眾** 的互動式心智圖。
選擇你的視角（投資者 / 知識工作者 / 一般消費者 / 公司決策者），地圖會**點亮該受眾的重點主題**，點主題即可看摘要、黃仁勳原句，並跳到對應的影片片段。

主軸：**從生成式 AI 到 Agentic AI，再到 Physical AI。**

## 開啟方式

| 方式 | 心智圖 | 內嵌影片 |
|---|---|---|
| **本機 http server（推薦）** | ✅ | ✅ 正常播放 |
| 直接雙擊 `file://` | ✅ | ⚠️ 改顯示「在 YouTube 開啟這一段」按鈕 |

推薦用本機 server（YouTube 內嵌需要有效的 http origin，`file://` 的 origin 為 `null` 會被擋）：

```bash
cd gtc_introduction
python3 -m http.server 8000
# 瀏覽器開 http://localhost:8000/gtc_taipei_2026_map.html
```

## 操作

- 拖曳空白處平移、滾輪縮放（React Flow 內建，右下有控制列與 minimap）
- 點中央四周的**視角節點** → 放射展開 13 個主題，核心主題會點亮（⭐ 重點）
- 點**主題節點** → 開詳情面板：摘要、關鍵名詞、黃仁勳原句、該視角解讀、影片片段
- 點中央「GTC Taipei 2026」可重置回選視角畫面

## 檔案

| 檔案 | 說明 |
|---|---|
| `gtc_taipei_2026_map.html` | 主成品（單一檔，React Flow + Lucide + Noto Sans TC/Space Grotesk，ESM CDN，免 build） |
| `transcript.srt` | 官方逐字稿（內容與時間戳的權威來源） |
| `keynote-timestamps.md` | 13 主題章節時間地圖（真實時間 + 黃仁勳原句） |
| `REFERENCES.md` | 全部參考來源（逐字稿為主 + 各媒體報導連結） |

## 註記

- **時間戳為逐字稿真實時間（非估計）。**
- 內容依據官方逐字稿，並以 2026/6 各媒體公開報導補充脈絡。
- 影片版權屬原頻道（電腦王阿達 @kocpc）：<https://www.youtube.com/watch?v=wzxc29ol3R0>
