# 114-2 資料探勘 期末專題

## 專題資訊

| 項目 | 說明 |
|------|------|
| 課程 | 114-2 資料探勘 |
| 組別 | 第 __ 組 |
| 專題名稱 | （請填入你們的專題名稱） |
| 組長 | （姓名 / GitHub 帳號） |
| 組員 | （姓名 / GitHub 帳號） |

---

## 專題說明

（請簡述你們的專題主題、分析目標與預期成果，約 3-5 句話）

---

## 專題要求

各組須運用本學期所學的資料探勘技術，針對一份與**海事或海洋**相關的資料集，完成完整的探勘分析流程。專題須包含以下環節：

1. **資料收集與描述**：說明資料來源、欄位定義、資料筆數與品質
2. **資料前處理與特徵工程**：遺漏值處理、異常值偵測、正規化、特徵選擇或萃取
3. **至少兩種探勘演算法的實作與比較**：從課程所學的演算法中選擇至少兩種進行建模
4. **模型評估**：使用適當的評估指標與交叉驗證
5. **結果視覺化與價值解讀**：將分析結果以圖表呈現，並解讀其實務意義

---

## 專題時程

| 週次 | 階段 | 說明 | 完成狀態 |
|------|------|------|---------|
| 第 3 週 | 分組與建立 Repo | 組長建立 Repo，邀請組員與老師 | ☐ |
| 第 4 週 | 個人題目探索 | 每人在 my-topics/ 提出 1-3 個題目構想 | ☐ |
| 第 5 週 | 決定題目與提案 | 繳交 proposal/proposal.md | ☐ |
| 第 6 週 | 提案審查 | 依教師建議修改提案 | ☐ |
| 第 7-8 週 | 前期研究 | 資料來源確認、初步資料收集與探索 | ☐ |
| 第 10-12 週 | 模型開發 | 資料清洗、特徵工程、模型訓練與調校 | ☐ |
| 第 13-15 週 | 進階分析 | 文字探勘、集群分析、結果視覺化 | ☐ |
| 第 16 週 | 整合測試 | 確保分析流程完整、修正問題 | ☐ |
| 第 17 週 | 準備發表 | 繳交期末報告和投影片 | ☐ |
| 第 18 週 | 期末發表 | 口頭報告 + Demo | ☐ |

---

## 資料夾結構

```
114-2_DM-G01/
├── README.md              ← 本檔案：專題說明與操作指引
├── .gitignore             ← Git 忽略規則
├── requirements.txt       ← Python 套件清單
├── proposal/              ← 專題提案
│   └── proposal.md
├── my-topics/             ← 個人題目探索
│   └── topic_template.md
├── data/                  ← 資料集
│   ├── raw/               ← 原始資料
│   ├── processed/         ← 處理後資料
│   └── README.md          ← 資料說明
├── src/                   ← Python 程式碼
│   ├── analysis/          ← 分析腳本
│   ├── model/             ← 模型訓練與評估
│   └── utils/             ← 共用工具函式
├── notebooks/             ← Jupyter Notebook
└── docs/                  ← 報告與投影片
    ├── report.md          ← 期末報告
    └── slides/            ← 發表投影片
```

### 各資料夾的用途

| 資料夾 | 放什麼 | 範例 |
|-------|-------|------|
| `data/raw/` | 原始資料檔案 | port_traffic_2024.csv |
| `data/processed/` | 清洗後的資料 | port_traffic_cleaned.csv |
| `src/analysis/` | 資料分析程式碼 | eda.py、preprocessing.py |
| `src/model/` | 模型訓練與評估 | train_model.py、evaluate.py |
| `src/utils/` | 共用工具函式 | helpers.py |
| `notebooks/` | Jupyter Notebook | 01_eda.ipynb、02_modeling.ipynb |
| `docs/report.md` | 期末報告 | 第 17 週繳交 |
| `docs/slides/` | 發表投影片 | 第 17 週繳交 |

---

## 評分標準

專題採用四維評分架構：

| 維度 | 評量對象 | 配分 | 評分方式 |
|------|---------|------|---------|
| 教師評分 | 整組 | 40% | 依下方細項給分 |
| 組間互評 | 整組 | 20% | 期末發表時各組互評 |
| 組內互評 | 個人 | 20% | Google 表單匿名評分 |
| AI 評分 | 個人 | 20% | Python 腳本分析 GitHub 數據 |

### 教師評分細項

| 項目 | 配分 | 說明 |
|------|------|------|
| 專題提案 | 5% | 題目合理性、可行性、創新性 |
| 資料品質與前處理 | 8% | 資料清洗完整、缺失值處理適當、特徵工程合理 |
| 探勘方法與模型 | 10% | 演算法選擇適當、模型評估完整、結果有洞察 |
| 視覺化與解讀 | 8% | 圖表清楚、分析結論有意義 |
| 程式碼品質 | 5% | 結構清楚、有註解、可讀性高 |
| 口頭報告與 Demo | 4% | 表達清楚、Demo 順暢、回答提問 |

### AI 評分重點

Python 腳本會自動分析每位組員在 GitHub 上的貢獻：

- Commit 次數與頻率
- Commit 時間分布（是否穩定開發，而非截止前趕工）
- 程式碼貢獻行數
- Commit 訊息品質（是否具描述性）
- 檔案覆蓋範圍（是否參與多個模組）

---

## 建議公開資料來源

| 資料來源 | 網址 |
|---------|------|
| 政府資料開放平臺 | data.gov.tw |
| 交通部航港局 | www.motcmpb.gov.tw |
| 海洋委員會海洋保育署 | www.oca.gov.tw |
| 中央氣象署 | www.cwa.gov.tw |
| 漁業署 | www.fa.gov.tw |
| MarineTraffic | www.marinetraffic.com |
| NOAA | www.noaa.gov |
| Copernicus Marine | marine.copernicus.eu |
| Kaggle | www.kaggle.com |

---

## 繳交項目 Checklist

- [ ] `proposal/proposal.md` 已填寫專題提案
- [ ] `data/README.md` 已填寫資料說明
- [ ] `src/` 中有完整的分析程式碼
- [ ] `notebooks/` 中有 Jupyter Notebook 分析過程
- [ ] `docs/report.md` 已完成期末報告
- [ ] `docs/slides/` 已上傳發表投影片
- [ ] `requirements.txt` 已更新實際使用的套件
- [ ] 本檔案 `README.md` 上方的專題資訊與說明已填寫

---

## 操作指引

> 以下內容說明從建立 Repo 到繳交報告的完整操作流程。

### 課程 Repo vs 專題 Repo

本課程有兩個 Repo，操作方式不同：

```
課程 Repo（114-2_DM）          專題 Repo（114-2_DM-G01）
├── 每週作業 → 學生 Fork + PR    ├── 專題開發 → 組員直接 Push
├── 個人繳交                     ├── 小組協作
└── 批改用                       └── 期末發表用
```

課程 Repo 是 Fork + PR 繳交作業；專題 Repo 是全組共用，直接 Push，不需要發 PR。

---

### 第 3 週：組長建立 Repo

以下步驟僅由**組長**操作。

**Step 1：從模板建立 Repo**

1. 打開專題模板：`https://github.com/pychang-ai/114-2_DM-project-template`
2. 點右上角綠色按鈕「**Use this template**」
3. 選擇「**Create a new repository**」
4. 填寫資訊：
   - Owner：選擇你自己的帳號
   - Repository name：`114-2_DM-G01`（替換為你的組別編號）
   - 選擇 **Public**
5. 點「**Create repository**」

**Step 2：邀請組員、老師、助教**

1. 進入你剛建立的 Repo，點上方「**Settings**」
2. 左側選單點「**Collaborators**」
3. 點「**Add people**」，依序邀請：
   - 所有組員的 GitHub 帳號（權限：Write）
   - 老師 `pychang-ai`（權限：Write）
   - 助教帳號（權限：Write）
4. 被邀請的人需到 GitHub 通知中點「**Accept invitation**」

**Step 3：通知組員**

在班級群組分享 Repo 網址，請組員接受邀請。

---

### 第 3 週：全體組員 Clone Repo

每位組員（含組長）把 Repo Clone 到自己的電腦：

```bash
git clone https://github.com/組長帳號/114-2_DM-G01.git
cd 114-2_DM-G01
```

使用 VS Code 也可以：按 `Ctrl+Shift+P` → 輸入 `Git: Clone` → 貼上 Repo 網址。

---

### 第 4 週：個人題目探索

每位組員各自提出 1-3 個題目構想。

1. 複製模板，用你的學號命名：
   ```bash
   cp my-topics/topic_template.md my-topics/A11218001_王小明.md
   ```
2. 編輯檔案，填入你的題目構想
3. 推送：
   ```bash
   git add my-topics/
   git commit -m "新增個人題目探索 - 王小明"
   git push origin main
   ```

在 GitHub 網頁操作也可以：到 `my-topics/` 點「Add file」>「Create new file」。

---

### 第 5 週：繳交專題提案

組內討論投票後，由**組長**填寫 `proposal/proposal.md` 並推送：

```bash
git add proposal/
git commit -m "繳交專題提案"
git push origin main
```

老師會在 `proposal.md` 底部的教師審查意見區填寫回饋。

---

### 第 7 週起：專題開發

**每次開發前先拉取最新版本：**

```bash
git pull origin main
```

**完成一段工作後推送：**

```bash
git add .
git commit -m "完成港口資料清洗與遺漏值處理"
git push origin main
```

**Commit 訊息撰寫建議：**

好的 Commit 訊息會影響 AI 評分，請寫清楚做了什麼：

```bash
# 好的訊息
git commit -m "新增港口船舶月統計折線圖"
git commit -m "完成缺失值處理與資料型態轉換"
git commit -m "使用隨機森林進行分類，測試準確率 0.87"

# 不好的訊息
git commit -m "update"
git commit -m "修改"
git commit -m "test"
```

**避免衝突的方式：**

分工時盡量負責不同的檔案，每次開發前先 `git pull`。如果 Push 時出現衝突：

```bash
git pull origin main          # 先拉取最新版本
# 打開檔案手動修改衝突區塊
git add .
git commit -m "解決合併衝突"
git push origin main
```

---

### 第 17 週：繳交報告

1. 完成 `docs/report.md` 期末報告
2. 將投影片放入 `docs/slides/`
3. 更新 `data/README.md` 的資料說明
4. 更新 `requirements.txt` 為實際使用的套件
5. 更新本檔案 `README.md` 上方的專題資訊與說明
6. 確認上方繳交項目 Checklist 全部打勾

---

## 常見問題

**Q：專題 Repo 需要發 PR 嗎？**
不需要。專題 Repo 是全組共用，直接 Push 到 main 即可。PR 只用在課程 Repo 的每週作業繳交。

**Q：我不是組長，可以建立和修改檔案嗎？**
可以。只要組長已邀請你為 Collaborator 且你已接受邀請，就有 Write 權限，可以直接 Push。

**Q：資料檔案太大怎麼辦？**
GitHub 單一檔案限制 100MB。如果資料太大，請在 `data/README.md` 中寫明下載方式，不要直接上傳。.gitignore 已設定忽略 `data/raw/` 中的 csv、xlsx、json 檔案。如果你的資料不大想直接上傳，可以把 .gitignore 中對應的行刪除。

**Q：可以用 Google Colab 的 Notebook 嗎？**
可以。在 Colab 完成分析後，點「檔案」>「下載」>「下載 .ipynb」，放到 `notebooks/` 資料夾中再 Push。

**Q：組員的 Commit 次數會影響成績嗎？**
會。AI 評分會分析每位組員的 Commit 次數、頻率、時間分布與程式碼貢獻量。請保持穩定的開發節奏，不要集中在截止前趕工。

**Q：忘記先 pull 就改檔案了怎麼辦？**
先 `git stash` 暫存修改，再 `git pull origin main` 拉取最新版本，最後 `git stash pop` 取回修改。如果有衝突就手動解決。
