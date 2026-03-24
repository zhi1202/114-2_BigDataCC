# CLAUDE.md — 巨量資料與雲端運算 AI 教學助手指南

## 一、課程定位

| 項目 | 內容 |
|------|------|
| 課程名稱 | 巨量資料與雲端運算 |
| 英文名稱 | Big Data Analytics and Cloud Computing |
| 學期 | 114 學年度第 2 學期 |
| 時間 | 週二 13:30–16:20 |
| 對象 | 日四技海資三甲 |
| 學校 | 國立高雄科技大學 海事資訊科技系 |
| 授課教師 | 張珀銀 助理教授 |
| 助教 | 邱麟翔 |
| GitHub Repo | pychang-ai/114-2_BigDataCC（public） |
| 作業繳交 | Fork + Pull Request |

本 repo 是學生面向的公開教學資源庫。CLAUDE.md 供 Claude.ai Project 和 Claude Code 讀取，用於輔助備課、出題、批改和回答學生問題。

## 二、教學目標與五大核心主題

1. **Linux 與雲端基礎**（Week 3–7）：Linux 操作、Bash Shell、AWS EC2
2. **虛擬化與容器技術**（Week 3, 13–14）：WSL、Docker、Dockerfile
3. **版本控制與協作開發**（Week 1–3）：Git、GitHub、Fork、PR
4. **Python 大數據分析**（Week 10–12, 15）：Pandas、Jupyter、Matplotlib
5. **AI 工具輔助開發**（Week 10–17）：Prompt Engineering、AI 輔助分析與部署

AI 使用核心原則：**先理解再使用**，確保學生具備獨立判斷與修正 AI 產出的能力。

## 三、Repo 目錄結構

```
114-2_BigDataCC/
├── CLAUDE.md                    ← AI 指引（本檔案）
├── README.md                    ← 學生用課程說明（完整18週進度、評分、專題）
├── .claude/                     ← AI 輔助設定（教師端）
│   ├── course-config.md         ← 課程週次設定與教材生成規則
│   └── grading-rules.md         ← 批改標準與評分細則
├── week01/ ~ week18/            ← 每週教材與作業說明
│   └── README.md                ← 本週學習目標、教材、作業要求
├── midterm/                     ← 期中考相關
├── final/                       ← 期末專題模板與說明
├── quizzes/                     ← 小考題庫
│   ├── quiz1/ ~ quiz4/
│   └── README.md
└── docs/                        ← 教師端教學文件
    ├── syllabus.md              ← 完整教學大綱
    └── weekly-checklist.md      ← 每週備課 checklist
```

## 四、週次進度速查表

| 週次 | 主題 | 工具導入 | 作業/考試 | 專題進度 |
|------|------|--------|--------|--------|
| 1 | 課程導論、Git/GitHub、ML 概述 | Git, VS Code | — | — |
| 2 | VS Code 與 GitHub 實作 | — | — | — |
| 3 | 虛擬化、Linux、SSH、Fork/PR | AWS EC2 | week03 | 分組+建 Repo |
| 4 | Linux 指令與 Bash 基礎 | — | week04, 小考1 | 個人題目探索 |
| 5 | nano、Shell Script | — | week05 | 決定題目+提案 |
| 6 | 使用者、權限、目錄結構 | — | week06 | 提案審查 |
| 7 | 套件管理、Web 伺服器 | Apache, PHP | week07 | 前期研究 |
| 8 | MySQL 資料庫 | MySQL | week08, 小考2 | 前期研究 |
| 9 | **期中考** | — | 期中考 | — |
| 10 | Python 環境與基礎語法 | Python, Miniconda | week10 | 資料分析 |
| 11 | Pandas 資料清洗 | Pandas, NumPy | week11 | 資料分析 |
| 12 | Jupyter 與資料視覺化 | Jupyter, Matplotlib | week12, 小考3 | 系統開發 |
| 13 | Docker 認識與安裝 | Docker Desktop | week13 | 系統開發 |
| 14 | Docker 操作與 Dockerfile | Dockerfile | week14 | Docker 部署 |
| 15 | Python 大數據綜合實作 | — | week15 | Docker 部署 |
| 16 | 機器學習與預訓練模型 | Keras, KerasNLP | week16, 小考4 | 整合測試 |
| 17 | Gradio AI 互動介面 | Gradio | 繳交期末報告 | 準備發表 |
| 18 | **期末專題發表** | — | 期末發表 | 口頭報告+Demo |

校曆第 1 週＝2/24 起算。期中考 Week 9（4/20–24）。清明假期 4/2、4/7。期末考 Week 17（6/8–12）。

## 五、作業與評分規則

### 評分比例

| 項目 | 比例 |
|------|------|
| 平時作業（Fork + PR） | 20% |
| 小考（4 次） | 20% |
| 期中考 | 20% |
| 期末專題 | 20% |
| 課堂參與 | 20% |

### PR 繳交規則

- 標題格式：`學號_姓名_weekXX`
- 每週作業放在對應 `weekXX/` 目錄
- 遲交規則：截止後 PR 標記 late，扣分依教師判斷

### 專題評分（四維架構）

教師評分 40% + 組間互評 20% + 組內互評 20% + AI 評分 20%

AI 評分透過 Python 腳本分析 GitHub 數據：commit 次數、時間分布、程式碼貢獻行數、commit 訊息品質、檔案覆蓋範圍、Docker 部署可行性。

## 六、技術環境

### AWS EC2 Linux 練習環境

| 項目 | 主機 1 | 主機 2 |
|------|--------|--------|
| IP | 54.151.244.27 | 54.255.61.68 |
| Port | 2201 | 2202 |
| 帳號/密碼 | 依帳號分配表 | 依帳號分配表 |

### 課程軟體

Git, VS Code, MobaXterm, Python/Miniconda, Docker Desktop

## 七、AI 使用政策

### 學生 AI 使用規範

- Week 10 前：不使用 AI 工具，先建立基礎能力
- Week 10 起：導入 AI 工具，遵循「先理解再使用」原則
- 所有 AI 輔助產出必須理解後才能提交
- 作業中使用 AI 需在 PR 說明中標註使用範圍

### AI 使用紅線

- 不可將整份作業交給 AI 完成後直接提交
- 不可複製 AI 產出而無法解釋其內容
- 小考和期中考禁止使用 AI

## 八、備課指引（Claude 輔助教師備課）

Claude 可協助教師完成以下備課工作：

### 8.1 每週教材生成

讀取 `.claude/course-config.md` 中的週次設定，生成：
- `weekXX/README.md`：本週學習目標、指令示範、練習題、作業要求
- 投影片大綱：按照「概念說明 → 指令示範 → 實作練習 → 作業佈達」四段式結構

### 8.2 教材生成規則

- 所有 Linux 指令範例必須可在課程 AWS EC2 環境上執行
- Python 範例使用 Miniconda 環境，套件限定課程清單內
- Docker 範例需考慮 AWS EC2 環境的資源限制
- 難度遞進：每週建立在前一週的基礎上
- 海事特色：範例和練習題儘量使用海事、海洋、港口相關資料集

### 8.3 備課 checklist

每週上課前確認：
1. weekXX/README.md 已更新
2. 練習用資料集或腳本已準備
3. AWS EC2 環境可正常連線
4. 上週作業 PR 已檢閱
5. 本週投影片已準備

## 九、出題指引（Claude 輔助教師出題）

### 9.1 小考出題

| 小考 | 範圍 | 題型 | 題數建議 |
|------|------|------|---------|
| 小考 1（W4） | Git、虛擬化、SSH、Linux 基本指令 | 選擇+簡答+實作 | 10–15 題 |
| 小考 2（W8） | Linux 進階、權限、Shell Script、Web、SQL | 選擇+簡答+實作 | 10–15 題 |
| 小考 3（W12） | Python、Pandas、Jupyter、視覺化 | 選擇+簡答+程式題 | 10–15 題 |
| 小考 4（W16） | Docker、Dockerfile、ML、預訓練模型 | 選擇+簡答+實作 | 10–15 題 |

出題原則：
- 60% 基礎觀念理解、20% 實際操作、20% 應用延伸
- 不出純記憶題，側重理解和實作
- 每次小考 30 分鐘內可完成

### 9.2 期中考出題

- 範圍：Week 1–8 全部內容
- 時間：一節課（50 分鐘）
- 題型：選擇 + 填空 + 簡答 + 指令實作
- 難度分布：易 40% / 中 40% / 難 20%

### 9.3 平時作業出題

每週作業放在 `weekXX/README.md` 的「作業」區塊，包含：
- 明確的操作步驟要求
- 預期輸出格式或截圖要求
- 繳交方式提醒（PR 標題格式）

## 十、批改指引（Claude 輔助教師批改）

### 10.1 PR 批改流程

1. 學生發 PR 到 pychang-ai/114-2_BigDataCC
2. 教師或 Claude 檢閱 PR 內容
3. 回饋方式：PR comment 或 review

### 10.2 批改標準

| 等級 | 分數 | 標準 |
|------|------|------|
| A | 90–100 | 完整正確，有額外探索 |
| B | 80–89 | 完整正確 |
| C | 70–79 | 大致正確，有小錯誤 |
| D | 60–69 | 部分完成或有明顯錯誤 |
| F | 0–59 | 未完成或抄襲 |

### 10.3 Claude 批改重點

- 檢查指令輸出是否正確
- 檢查 commit 訊息是否有描述性
- 檢查檔案結構是否符合要求
- 檢查 Shell Script 是否可執行
- 對 Python 程式碼：檢查邏輯、風格、效率
- 回饋語氣：鼓勵為主，指出問題並給出改善建議

### 10.4 批改回饋模板

```markdown
## 作業批改回饋

**學生**：{學號}_{姓名}
**週次**：Week {XX}
**成績**：{A/B/C/D/F}

### 完成度
- [ ] 題目 1：{通過/需修正}
- [ ] 題目 2：{通過/需修正}

### 優點
- {具體優點}

### 改善建議
- {具體建議}

### 補充學習資源
- {相關參考連結}
```

## 十一、與 time-master 的關係

本 repo 的課程進度透過以下方式回報到 time-master 工作管理系統：

- **time-master/state/weekly-focus.md**：本週上課主題和待辦
- **time-master/reference/courses.md**：課程基本資訊
- **time-master/state/repo-tracker.md**：repo 總覽

time-master 追蹤「第幾週上什麼」和「作業是否批改完」，不管教材細節。教材細節由本 repo 和對應的 Claude.ai Project 管理。

由於本 repo 是公開的，不需要從 time-master 同步 context/，也不存放任何敏感資訊。

## 十二、commit 規範

| 前綴 | 用途 | 範例 |
|------|------|------|
| `material:` | 新增或更新教材 | `material: week05 Shell Script 教材` |
| `assignment:` | 新增或更新作業 | `assignment: week05 作業說明` |
| `quiz:` | 小考相關 | `quiz: 小考1 題目與解答` |
| `fix:` | 修正錯誤 | `fix: week03 SSH 連線指令修正` |
| `docs:` | 文件更新 | `docs: 更新課程進度表` |
| `config:` | 設定調整 | `config: 更新 .claude/ 設定` |

## 十三、禁止事項

1. **不要在本 repo 放學生成績或個人資料**：本 repo 是公開的
2. **不要在本 repo 放小考答案**：答案放在 Claude.ai Project Knowledge
3. **不要在本 repo 放 AWS 密碼或 Token**：帳號分配表不進 GitHub
4. **不要修改學生的 PR 內容**：只做 comment 或 review
5. **不要刪除已發布的教材**：學生可能已 fork
