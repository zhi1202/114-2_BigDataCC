# 課程週次設定與教材生成規則

> 用途：Claude 生成每週教材時的參考設定

## 教材生成模板

每週 README.md 結構：

```markdown
# Week XX：{主題}

## 本週學習目標

完成本週課程後，你將能夠：
1. {目標 1}
2. {目標 2}
3. {目標 3}

## 課程內容

### {主題 A}
{概念說明 + 指令示範}

### {主題 B}
{概念說明 + 指令示範}

## 課堂練習

{2–3 個課堂練習題}

## 本週作業

### 繳交方式
在你的 Fork 中建立 `weekXX/` 資料夾，完成後發 PR。
PR 標題：`學號_姓名_weekXX`

### 作業內容
{具體作業題目}

### 截止日期
{下次上課前}
```

## 週次詳細設定

### Week 1–2：Git 與開發環境

教材重點：Git 基本操作、VS Code 設定、GitHub 帳號、SSH key
練習環境：學生本機
海事元素：無，專注於工具建立

### Week 3–5：Linux 基礎

教材重點：SSH 連線、基本指令、目錄操作、nano、Shell Script
練習環境：AWS EC2（ssh student@IP -p port）
海事元素：用海洋資料檔案名稱作為練習素材

### Week 6–8：Linux 進階與 Web

教材重點：權限管理、套件管理、Apache、PHP、MySQL
練習環境：AWS EC2
海事元素：海洋氣象資料庫作為 SQL 練習

### Week 9：期中考

不需生成教材

### Week 10–12：Python 資料分析

教材重點：Python 基礎、Pandas、Jupyter、Matplotlib
練習環境：AWS EC2 + Miniconda
海事元素：港口吞吐量、AIS 船舶資料、海洋氣象資料
AI 工具：Week 10 起導入 Prompt Engineering

### Week 13–14：Docker

教材重點：Docker 概念、安裝、基本操作、Dockerfile
練習環境：AWS EC2 或本機 Docker Desktop
海事元素：部署海事資料分析應用

### Week 15–17：綜合實作與 AI

教材重點：完整分析流程、機器學習、Gradio 部署
練習環境：AWS EC2 + Docker
海事元素：期末專題以海事為主題
AI 工具：AI 輔助完整開發流程

### Week 18：期末發表

不需生成教材，準備評分表

## 教材品質標準

1. 指令範例必須在 AWS EC2 Ubuntu 環境可執行
2. Python 範例使用 Python 3.10+ 語法
3. 每個概念先說明「為什麼需要」再教「怎麼做」
4. 每週教材閱讀時間控制在 20 分鐘內
5. 練習題有明確的預期輸出或驗證方式
