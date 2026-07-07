# 基礎學習網站模板

這個資料夾提供一套可重用的靜態學習網站模板，適合製作：

- 1 個首頁 + 多個課程頁
- 教學文章 + 生活例子 + 小測驗
- 不需要後端、不需要打包工具的純 HTML 網站

## 檔案用途

- `home-template.html`：首頁模板，包含主視覺標題、簡介、歡迎說明框、課程卡片 grid。
- `lesson-template.html`：課程頁模板，包含返回首頁、課程標題、內容章節、提示框、2 題即時回饋測驗。

## 使用方式

1. 複製 `home-template.html`，改名為 `index.html`。
2. 複製 `lesson-template.html`，依課程數量改名，例如 `course1.html`、`course2.html`。
3. 修改首頁卡片中的課程名稱、簡介、連結和學習重點。
4. 修改課程頁中的標題、核心概念、生活例子和測驗題目。
5. 測驗選項用 `data-correct="true"` 標示正確答案，用 `data-explain` 填入答案解析。

## 建議結構

```text
your-site/
├── index.html
├── course1.html
├── course2.html
├── course3.html
└── ...
```

## UI 風格

這份模板採用簡潔教學網站風格：

- 深藍漸層首頁 header
- 白色卡片式課程列表
- 單欄閱讀式課程頁
- 深藍標題底線與章節左側藍線
- 淡藍提示框
- 表單式測驗互動

整套模板是純 HTML，每個檔案都包含自己的 `<style>` 與 `<script>`，方便直接複製使用。
