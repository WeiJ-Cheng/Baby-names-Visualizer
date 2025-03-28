# Baby Names Trend Visualizer 👶📈

## 📖 程式介紹

這是一個使用 Python 與 Tkinter 製作的圖形化應用程式，允許使用者輸入名字並視覺化顯示該名字在 1900~2020 間的流行趨勢。

---

## ✅ 功能

- 🔍 **即時搜尋**：輸入名字，即可查詢 1900 到 2020 的母婦名第名趨勢
- 📈 **折線圖顯示**：通過 Tkinter Canvas 擺顯各名字各年度的評等變化
- 📌 **每個點勾有名字 + 名次標示**，若無資料則顯示 *
- 🎨 **多名字支援**：同時顯示多個名字資料，並以顯著的顏色分別
- 🧪 **不分大小寫搜尋**：輸入 aLiCe 也會補正為 Alice 搜尋

---

## 💻 使用技術

| 類別 | 技術說明 |
|--------|------------------|
| 程式語言 | Python 3.x |
| GUI | Tkinter (Canvas, Entry, Label) |
| 資料解析 | Dictionary (層級結構：`{name: {year: rank}}`) |
| 圖形顯示 | `canvas.create_line()`, `canvas.create_text()` |
| 多顏色 | `COLORS[i % len(COLORS)]` 轉換顏色 |

---
📷 範例圖片

幫助你更好地理解程式圖形結果，下面是兩張操作畫面範例：

範例 1



範例 2

---
## 📁 資料檔

本項目使用已處理好的網路母婦名名第檔，格式为:

```
data/full/baby-1900.txt
```
每一檔包含：
```
1900
1,John,Mary
2,William,Helen
...
```

---

## 🚀 啟動方式

確保你已經安裝 Python 3.x，使用系統內建的 tkinter 就可以啟動：

```bash
python3 babygraphics.py
```

---

## 🌟 其他

- 指定名字同時顯示多條折線，以顏色分別
- 搜尋核心使用 `babynames.search_names()`
- GUI 介面由 `babygraphicsgui.py` 提供

---

📙 Created for learning and visualization purpose, based on Stanford CS106AP 寫作執行功能之模範。
