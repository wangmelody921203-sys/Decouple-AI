# Week 10 實作導引（可直接照做）

## 你現在要做的順序
1. 先完成 Section 0（環境準備）
2. 再做 Section 1（BASELINE 截錄）
3. 做 Section 2（洞見）
4. 做 Section 3（升級規格）
5. 做 Section 4（實際改造）
6. 做 Section 5（v1 vs v2 對照）
7. 做 Section 6（v2 更新 + 反思）

---

## Section 0｜環境準備（5 min）
### 0-1 檢查 Week 9 是否在 GitHub
如果還沒推上去，對 Gemini CLI 下這句：

我要把我的公司 repo 推到我的 GitHub。請從建 repo 到 push 一次到位，過程中需要什麼資訊就問我。我的 GitHub 帳號是 [你的帳號]

### 0-2 重組資料夾（Week 9 產出歸檔）
請把你目前 week9 根目錄的這些檔案移到 /w9/：
- brief.md
- deliverable.md
- reflection.md
- company-screenshot.png（如果有）

再建立 /w10/（如果你打算在 week9 repo 內做 Week10 產出）。

---

## Section 1｜BASELINE 截錄（5 min）
1. 把你課前 v1 公司簡介貼到 `notes.md`。
2. 把對齊型客戶 brief 填好 4 個空格，存到 `aligned-client-brief.md`。
3. 對 Gemini CLI 下指令跑 v1 output，輸出到 `client-brief-v1-output.md`。

建議指令：

請用我現在這個版本（main branch）的公司、處理以下這份客戶 brief：
@/w10/aligned-client-brief.md
請按你公司原本的 COO 工作流跑完整個流程、
把最終 deliverable 存成 /w10/client-brief-v1-output.md。
完成後告訴我這份 deliverable 的長度跟主要章節結構。

---

## Section 2｜課堂洞見萃取（10 min）
打開 `insights.md`，用你自己的話填完 4+1 鏟子與「最戳的一句」。

---

## Section 3｜升級規格書（30 min）
打開 `upgrade-spec.md`，依模板完成 A-E 區、specialist 改造、workflow 改造。

硬條件：至少新增 1 個「只有 AI 在場才存在」的 specialist 或 workflow。

---

## Section 4｜實際改造（30-45 min）
在 Gemini CLI 依序做：
1. 開 branch `w10-upgrade`
2. 套用 `upgrade-spec.md` 改 `spec.md`
3. commit
4. 改 specialist
5. 新增原生型 specialist（必做）
6. 輸出 `.agent/` 結構（tree）
7. merge 回 main、打 tag `v2`、push

---

## Section 5｜同一客戶 brief 的改造前後對照（30 min）
1. 用新版 main 再跑一次同份 brief。
2. 輸出到 `client-brief-v2-output.md`。
3. 並列比較 v1 與 v2。
4. 在 `reflection.md` 填四題。

---

## Section 6｜v2 更新 + 反思（10 min）
1. 在 `v2-summary.md` 填新版公司簡介。
2. 在 `reflection.md` 最後補「我之前看不見，現在看見了什麼」。
3. commit + push。

---

## 最後繳交清單（對照 checklist.md）
完成所有檔案後，打開 `checklist.md` 自我驗收。