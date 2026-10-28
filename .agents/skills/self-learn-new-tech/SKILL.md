---
name: self-learn-new-tech
description: >-
  Generates structured, scenario-driven self-learning materials and interactive HTML guides for any new technology topic. Use this skill whenever the user wants to learn a new technology (e.g., Git, Docker, Next.js, SQL, Vector DB) or asks to produce beginner-friendly learning roadmaps, especially tailored for AI-first developers (Vibe Coders).
---

# Self-Learn New Tech (新技術自學與互動教材生成工作流)

本 Skill 定義了一套標準化的「新技術自學與互動教材開發方法論」。無論未來的主題是 **Docker、SQL、Next.js、Vector DB 或 CI/CD**，皆依循此 SOP 迅速產出兼具直覺比喻、防呆防護、互動演練與影音推薦的高品質繁體中文自學教材。

---

## 核心設計理念 (Core Principles)

1. **以學習者視角為中心 (Persona-First)**：
   * 針對 **Vibe Coder（AI 協作開發者）**，核心不是死背每條語法或指令，而是掌握「底層心智模型」、「如何指揮 AI 協作」、「如何防止 AI 改壞程式碼」以及「如何設立資安防線」。
2. **直覺比喻降維 (Metaphor-Driven)**：
   * 將抽象名詞轉化為生活常識或遊戲機制（例如：Commit = 存檔點、Branch = 平行宇宙、.gitignore = 機密防護網）。
3. **情境痛點導向 (Scenario-Based)**：
   * 不按功能手冊線性排列，改由使用者最容易踩坑的「災難現場」與「高頻場景」切入（例如：「救命！AI 把代碼改爛了」、「API 密鑰如何不外洩」）。
4. **一鍵上手與互動驗證 (Actionable & Interactive)**：
   * 提供具備「一鍵複製內容」按鈕的指令區塊與「Try This 實戰演練」檢查機制，大幅降低動手門檻。

---

## 標準產出 SOP (6 步工作流)

### 步驟 1：學習者畫像分析 (Persona Profiling)
* 確認目標受眾背景（如：零基礎新手、Vibe Coder、跨領域產品經理）。
* 釐清痛點：初學者在接觸該技術時最害怕什麼？最容易在哪個環節卡關或造成破壞？

### 步驟 2：核心觀念的生活化比喻 (Mental Model & Metaphors)
* 提煉該技術的 3~4 個核心元件，並為每個元件設計一個生活化或遊戲化比喻。
* 繪製高層次流動圖（SVG / 流程圖），視覺化資訊或狀態的流轉過程。

### 步驟 3：高頻實戰情境規劃 (Core Scenarios)
設計 4~6 個真實高頻使用情境，每個情境包含：
* **為什麼需要這個步驟？**
* **指令 / 代碼區塊**（附帶一鍵複製按鈕）。
* **AI Prompt 範例**（教使用者如何向 Cursor、Antigravity 或 Claude 提問以完成該任務）。

### 步驟 4：防護罩與災難急救手冊 (Safety & Disaster Recovery)
* 挑出初學者最常犯的重大致命錯誤（例如：敏感資訊外洩、程式碼覆蓋丟失、環境污染）。
* 提供對應的「黃金防禦法則」與「一鍵還原急救指令」。

### 步驟 5：精選影音與互動學習庫 (Multi-Modal Curation)
* **YouTube 推薦**：搜尋評分高、畫質佳、解說清楚的繁體中文或雙語影音教學。
* **互動沙盒**：找出該技術領域內最優秀的線上遊戲化學習工具（例如 Git 領域的 *Learn Git Branching*）。
* **權威文檔與速查工具**：官方文檔、開源書籍、自動生成工具。

### 步驟 6：互動式 HTML 教材生成 (Interactive Artifact Deliverable)
將以上內容編排為現代化輕量風格的單一純 HTML 檔案：
* **頁籤分頁 (Tab Navigation)**：讓使用者專注於單一章節，避免無限滾動疲勞。
* **淺色簡約設計 (Light-Color Aesthetic)**：採用 Slate / Indigo / Emerald 等溫潤對比配色。
* **內嵌 SVG 資訊圖表 (Infographics)**：無須外部圖片依賴，向量清晰。
* **「Try This」演練卡片與進度條**：每單元包含具體操作與打勾完成狀態。
* **一鍵複製內容按鈕 (Copy to Clipboard)**：每個指令與 Cheat Sheet 皆具備一秒複製功能。

---

## 教材樣板結構 (HTML Artifact Architecture)

```html
<!DOCTYPE html>
<html lang="zh-TW">
<head>
  <script src="https://www.gstatic.com/antigravity/web/dev/tailwindcss.min.js"></script>
  <!-- 頁籤樣式與按鈕動畫 -->
</head>
<body class="bg-slate-50 text-slate-800">
  <header>標題、學習進度條、章節頁籤 (Tabs)</header>
  <main>
    <!-- Tab 1: 觀念與生活化比喻 + 核心 SVG 資訊圖解 -->
    <!-- Tab 2: 環境建置與第一個里程碑實作 + Try This #1 -->
    <!-- Tab 3: 防護罩（資安意識與災難急救回滾術）+ Try This #2 -->
    <!-- Tab 4: 進階實用情境（平行分支/實驗/模組化）+ Try This #3 -->
    <!-- Tab 5: 雲端整合/部署發布 + Try This #4 -->
    <!-- Tab 6: 精選 YouTube 影音與互動沙盒資源庫 -->
    <!-- Tab 7: 常用指令急救速查卡 (Cheat Sheet) -->
  </main>
  <!-- 一鍵複製 Clipboard JS 與 Toast 通知 -->
</body>
</html>
```
