# /pulse-check

## 目的
在交付前快速檢查三件事：成本、幻覺風險、客戶自操作能力。

## 檢查清單
1. 成本：是否有清楚的 token 成本基線與優化幅度。
2. 風險：是否有至少 3 個高機率錯誤情境與對應防呆。
3. 自操作：客戶是否可在 15 分鐘內理解與操作核心流程。

## 輸出模板
- cost-status: pass | warn | fail
- hallucination-status: pass | warn | fail
- self-serve-status: pass | warn | fail
- blockers: 目前阻塞點
- fix-next: 下一步修正
