# Week 11 實作導引（延續 Week 10）

## 0. 本週目標
1. 驗證公司可在 agy 正常運作。
2. 你以老闆身分定義客戶 brief。
3. 讓公司依 brief 產生服務方案，並做判斷。

## 0.5 安裝與登入 Antigravity CLI（若尚未安裝）
你的環境目前可用指令是 `antigravity`（等價於課堂文件中的 `agy`）。

請先在 terminal 執行：

```bash
curl -fsSL https://antigravity.google/cli/install.sh | bash
```

安裝後執行：

```bash
antigravity
```

第一次會開瀏覽器要求登入 Google，完成授權後再回來做第 1 步。

## 1. 遷移驗證（先做）
在 repo 根目錄執行：

```bash
antigravity
```

第一句可輸入：

```text
請依照 spec.md 描述的公司結構，
簡短介紹你（COO）和你的 specialists 各是誰，
以及你們服務的客戶類型。
```

若回答正確，再建立遷移標記：

```bash
echo "Migrated to Antigravity CLI on 2026-06-18" > w11/migration-confirmed.md
```

## 2. 寫 client brief（你當老闆）
打開 `w11/client-brief.md`，先填「五格框架」，再寫 50 字 brief。

完成後可對 Antigravity CLI 輸入：

```text
請讀取 w11/client-brief.md 這份客戶需求書，
依照 spec.md 描述的公司能力，
為這位客戶設計一份具體服務方案。
服務方案請輸出到 w11/service-design-v1.md
```

## 3. 老闆判斷（必做）
讀完 `w11/service-design-v1.md`，回到 `w11/reflection.md` 填完四題判斷。

如果你判斷仍不足，可再跑一輪：

```text
請根據我在 w11/reflection.md 提到的不足點，
提出修正版方案並輸出到 w11/service-design-v2.md
```

## 4. Git 收尾

```bash
git add w11/ .agent/ spec.md
git commit -m "W11: define client, serve client, reflect"
git tag v3
git push origin main --tags
```

最後檢查 tags：

```text
https://github.com/<你的帳號>/<你的repo>/tags
```
