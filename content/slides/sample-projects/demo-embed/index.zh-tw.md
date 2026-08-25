---
title: "範例：Markdown 搭配嵌入 HTML 網頁"
date: 2026-08-25
categories: ["範例作品集"]
access: public
---

## 簡介

這是一個範例頁面，展示如何在 **Markdown 內容** 中同時嵌入 `static/` 資料夾內的互動式 HTML 網頁。

你可以在這裡正常撰寫 Markdown — 標題、清單、程式碼區塊、連結、圖片 — 任何你需要的內容。

## 嵌入投影片：If 條件判斷

以下是直接嵌入在此 Markdown 頁面中的「If 條件判斷」互動投影片：

{{< embed-html src="/slides-html/coding-basics/if/index.html" height="600px" >}}

## 繼續撰寫 Markdown 內容

如你所見，嵌入的 HTML 網頁會與其他內容一起排列顯示。你可以在嵌入區塊後繼續撰寫。

### 重點整理

- 你可以自由地混合 Markdown 文字與嵌入的 HTML 網頁
- `embed-html` shortcode 支援自訂 `height`、`width`，以及控制是否顯示全螢幕按鈕
- 每個嵌入的網頁都有獨立的全螢幕按鈕，方便觀看

## 另一個嵌入範例：Switch 語法

這是另一個嵌入不同投影片的範例：

{{< embed-html src="/slides-html/coding-basics/switch/index.html" height="500px" >}}

## Shortcode 參數說明

| 參數          | 預設值     | 說明                              |
|--------------|-----------|-----------------------------------|
| `src`        | （必填）   | `static/` 資料夾內的 HTML 檔案路徑 |
| `height`     | `600px`   | iframe 高度                        |
| `width`      | `100%`    | 容器寬度                           |
| `fullscreen` | `true`    | 是否顯示全螢幕按鈕（`true`/`false`）|

## 不顯示全螢幕按鈕的範例

{{< embed-html src="/slides-html/coding-basics/oop/index.html" height="400px" fullscreen="false" >}}

---

以上就是完整的展示！這個頁面示範了 Markdown 與嵌入 HTML 如何無縫共存。
