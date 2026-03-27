# 🏔️ CryptoExpedition

> **A Multi-AI Agent Crypto Trading System**
> 6 位 AI 角色組成遠征隊，在加密貨幣市場中協作、辯論、進化。

<div align="center">

**分析師** · **守護者** · **批判者** · **研究員** · **網格師** · **進化者**

*「不是一個 AI 在交易，而是一個 AI 團隊在討論該不該交易。」*

</div>

---

## 🌍 故事的開始

很久以前，有一片名為 **Crypto** 的古老大陸。

這片大陸上遍佈著珍貴的寶藏，但也潛伏著危險的怪物——

<img src="assets/monster_black_swan.png" width="40" align="left" style="margin-right:8px"> **黑天鵝** — 無預警時從天而降，一口吞噬所有利潤。

<br clear="both">

<img src="assets/monster_fake_breakout.png" width="40" align="left" style="margin-right:8px"> **假突破幽靈** — 引誘冒險者踏入陷阱，看似突破卻瞬間反轉。

<br clear="both">

<img src="assets/monster_low_vol_spider.png" width="40" align="left" style="margin-right:8px"> **低波動蜘蛛網** — 用無盡的盤整困住旅人，進退兩難慢性失血。

<br clear="both">

<img src="assets/monster_emotion_tsunami.png" width="40" align="left" style="margin-right:8px"> **情緒海嘯** — 恐慌與貪婪的巨浪，席捲一切理智。

<br clear="both">

<img src="assets/monster_overfit_skull.png" width="40" align="left" style="margin-right:8px"> **幻術士** — 用過去的假象施展幻術，回測完美實戰慘敗。

<br clear="both">

<img src="assets/monster_sl_zombie.png" width="40" align="left" style="margin-right:8px"> **止損陷阱** — 在暗處悄悄收緊止損繩索，讓冒險者明明方向對卻掉入陷阱。

<br clear="both">

無數獨行的冒險者來了又走，帶著傷痕離開。

直到有一天，六位各懷本領的英雄決定**組隊遠征**——不再獨自戰鬥，而是各司其職，透過**布告欄**分享情報，用**否決權**阻止衝動，讓**研究員**不斷發現新的戰術，由**國王**審視全局。

這就是 **CryptoExpedition** 的故事。

---

## 📖 概念

大多數 AI 交易系統是**單一模型決策**——一個 AI 看數據、下判斷、執行交易。

CryptoExpedition 不同。它是一個 **Multi-Agent 協作系統**，每位 AI 角色有自己的專業、性格和否決權，透過共享**布告欄**溝通，像一支遠征隊一樣在市場中前進。

```
                    ┌─────────────┐
                    │   進化者 👑   │  ← 國王，每天審視全局
                    │  系統全局評估  │
                    └──────┬──────┘
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
  ┌─────┴─────┐    ┌──────┴──────┐    ┌──────┴──────┐
  │ 分析師 🔮  │    │  研究員 🧪   │    │  網格師 ♟️  │
  │ 市場方向判斷 │    │ 假設生成驗證  │    │ 網格參數優化  │
  └─────┬─────┘    └──────┬──────┘    └─────────────┘
        │                 │
        │     ┌───────────┴───────────┐
        │     │    📋 布告欄（共享）     │
        │     │ 各角色即時觀點+仲裁規則  │
        │     │ 所有人都能讀寫          │
        │     └───────────────────────┘
        │ 訊號          ▲
        ▼               │ 讀取
  ┌─────────────┐     通過      ┌─────────────┐
  │  批判者 ⚖️   │ ──────────→  │   守護者 🛡️  │
  │ 進場否決權   │              │ 持倉管理保護  │
  └─────────────┘              └─────────────┘
        │ 否決
        ▼
     不交易
```

---

## 🎭 六位角色

### 🔮 分析師 (Analyst)

<img src="assets/analyst.png" width="80" align="left" style="margin-right:16px">

> *「我負責看盤，告訴大家該做多還是做空。」*

- **職責**：每 10 分鐘分析市場數據，產出方向訊號
- **工具**：技術指標、9 大策略投票、新聞情緒、多時間框架分析
- **權限**：建議權（不能直接下單）
- **模型**：Claude Sonnet

<br clear="both">

### 🛡️ 守護者 (Position Manager)

<img src="assets/guardian.png" width="80" align="left" style="margin-right:16px">

> *「我保護你的倉位，管好止損止盈。」*

- **職責**：每 3 分鐘評估持倉健康狀態
- **工具**：即時價格、ATR、RSI、MACD
- **權限**：可調整止損止盈，但不能在分析師同方向高信心時平倉
- **模型**：Claude Haiku（快速回應）

<br clear="both">

### ⚖️ 批判者 (Critic)

<img src="assets/critic.png" width="80" align="left" style="margin-right:16px">

> *「我是進場的守門員，不通過我不准交易。」*

- **職責**：每次進場前挑戰分析師的判斷
- **權限**：**否決權**（必要條件，不是建議）
- **特殊**：批判者失敗 = 強制不交易（安全優先）
- **模型**：Claude Haiku

<br clear="both">

### 🧪 研究員 (Researcher)

<img src="assets/researcher.png" width="80" align="left" style="margin-right:16px">

> *「我發現新規律，驗證後變成投票策略。」*

- **職責**：產生市場假設 → 追蹤 7 天 → 驗證 → 晉升為新策略
- **三階段上線**：Shadow（0 影響）→ 低權重 → 正常權重
- **淘汰機制**：勝率 < 35% 自動退場

<br clear="both">

### ♟️ 網格師 (Grid Master)

<img src="assets/evolver.png" width="80" align="left" style="margin-right:16px">

> *「我優化網格的格距和範圍，低波動時出動。」*

- **職責**：低波動時啟動網格交易，自動優化參數
- **工具**：ATR、歷史績效、Claude 進化建議

<br clear="both">

### 👑 進化者 (Evolver)

<img src="assets/meta.png" width="80" align="left" style="margin-right:16px">

> *「我是國王，每天審視全局找出最弱的環節。」*

- **職責**：每天一次系統全局評估
- **輸出**：系統成熟度評分、最弱環節、進化提案
- **權限**：不直接改 code，產出建議供人工審核
- **模型**：Claude Sonnet

<br clear="both">

---

## ⚔️ 遠征路上的怪物

市場不是空白地圖。遠征隊每天都在跟這些怪物戰鬥：

<table>
<tr>
<td width="80"><img src="assets/monster_black_swan.png" width="64"></td>
<td><b>🦢 黑天鵝</b><br>閃崩、暴漲、突發事件 — 一口吃掉所有利潤<br><i>應對：守護者（即時止損）+ 風控硬止損 25%</i></td>
</tr>
<tr>
<td><img src="assets/monster_fake_breakout.png" width="64"></td>
<td><b>👻 假突破幽靈</b><br>看似突破卻反轉 — 方向對但被止損掃出<br><i>應對：分析師（多時間框架確認）+ 動態 ATR 止損</i></td>
</tr>
<tr>
<td><img src="assets/monster_low_vol_spider.png" width="64"></td>
<td><b>🕷️ 低波動蜘蛛網</b><br>盤整行情，上下震盪 — 反覆進出，慢性失血<br><i>應對：網格師（切換網格策略）+ Deadzone 過濾</i></td>
</tr>
<tr>
<td><img src="assets/monster_emotion_tsunami.png" width="64"></td>
<td><b>🌊 情緒海嘯</b><br>FOMO、恐慌、極端情緒 — AI 被情緒誤導<br><i>應對：批判者（否決衝動交易）+ Regime 禁止機制</i></td>
</tr>
<tr>
<td><img src="assets/monster_overfit_skull.png" width="64"></td>
<td><b>💀 過擬合骷髏</b><br>回測完美但實戰慘敗 — 策略只適用過去<br><i>應對：研究員（三階段上線）+ Shadow Trading 驗證</i></td>
</tr>
<tr>
<td><img src="assets/monster_sl_zombie.png" width="64"></td>
<td><b>🧟 SL 殭屍</b><br>止損被反覆收緊到幾乎為零 — 方向對卻秒掃<br><i>應對：最小寬度保護 + tighten cooldown + 仲裁機制</i></td>
</tr>
</table>

> *每一隻怪物都是我們真實遇到的 bug 或虧損。每一個防禦機制都是被打敗後設計出來的。*

---

## 🏗️ 系統架構

```
┌─────────────────────────────────────────────────────┐
│                    交易系統架構                        │
├─────────────────────────────────────────────────────┤
│                                                     │
│  ┌─────────┐  ┌──────────┐  ┌─────────┐           │
│  │DataCollect│→│ 9 Voters │→│ Claude   │           │
│  │市場數據   │  │策略投票   │  │分析+訊號 │           │
│  └─────────┘  └──────────┘  └────┬────┘           │
│                                   │                 │
│                    ┌──────────────┼────────┐        │
│                    │              │        │        │
│              ┌─────┴─────┐ ┌─────┴────┐  │        │
│              │  Critic    │ │ Bot 過濾  │  │        │
│              │  否決/通過  │ │品質+風控  │  │        │
│              └─────┬─────┘ └─────┬────┘  │        │
│                    │             │        │        │
│                    └──────┬──────┘        │        │
│                           │               │        │
│                    ┌──────┴──────┐        │        │
│                    │  執行/Paper  │        │        │
│                    │  Trade       │        │        │
│                    └──────┬──────┘        │        │
│                           │               │        │
│              ┌────────────┴───────┐       │        │
│              │  Price Monitor     │       │        │
│              │  即時監控 (10秒)    │       │        │
│              │  SL/TP/Trail/Lock  │       │        │
│              └────────────────────┘       │        │
│                                           │        │
│  ┌──────────────────────────────────────┐ │        │
│  │         Agent 共享布告欄 📋              │ │        │
│  │  各角色即時觀點 + 仲裁規則             │◄┘        │
│  └──────────────────────────────────────┘          │
│                                                     │
│  ┌──────────────────────────────────────┐          │
│  │         進化系統 🧬                    │          │
│  │  假設引擎 → 驗證 → 動態 Voter          │          │
│  │  Shadow Trading → Deadzone 自適應     │          │
│  │  每日深度覆盤 → 參數自動調整           │          │
│  └──────────────────────────────────────┘          │
│                                                     │
└─────────────────────────────────────────────────────┘
```

---

## 🧠 核心設計理念

### 1. 分層否決權
```
Layer 1: 分析師 → 建議方向（僅建議）
Layer 2: 批判者 → 否決權（必要條件）
Layer 3: 品質過濾 → Deadzone、Regime、ATR
Layer 4: 守護者 → 持倉管理（受分析師約束）
```
任何一層說「不」，交易就不會發生。

### 2. Agent 績效追蹤
每位角色的建議都被記錄並與實際結果比對：
- 分析師：方向判斷準確率
- 守護者：平倉建議是否正確（平倉後價格是否繼續有利）
- 批判者：否決的交易如果進場了會怎樣

績效差的角色自動降低權重。

### 3. 自適應進化
```
每日覆盤 → 發現 pattern → 產生假設 → Shadow 驗證
    → 正確率 >60% → 三階段上線（Shadow→低權重→正常）
    → 勝率 <35% → 自動淘汰
```

系統不需要人工調參，會自己學習哪些策略有效。

### 4. Confidence Deadzone
分析數據發現某些信心區間表現差（例如 40-60%），自動封鎖該區間。被封鎖的交易以 **Shadow Trade** 繼續追蹤虛擬損益，表現恢復後自動解封。

### 5. 共享布告欄

<img src="assets/blackboard.bmp" width="400">

所有角色透過布告欄溝通即時觀點：
```
[分析師] ↓ 做空 conf=65% "MTF 全空"  (5m前)
[守護者] 持有 止損=1.0%  (2m前)
[批判者] 通過  (10m前)
[研究員] 3 假設追蹤中  (1h前)
```
守護者讀到分析師仍看空，就不會輕易平掉空單。

---

## 📊 出場管理

不是簡單的固定止損。多層動態出場系統：

```
入場 止損 ~2%（Claude 根據波動率決定）
  │
  ├─ 浮盈 > 1.5×ATR → Breakeven（止損移到成本 ±0.5×ATR）
  │
  ├─ 浮盈 > 1×ATR → Lock2（止損鎖住 0.5×ATR 利潤）
  │
  ├─ 浮盈 > 0.5×ATR → Profit Trail 啟動（回撤 0.3×ATR 出場）
  │
  ├─ 有浮盈 + 止損距現價 <0.3% → 最小寬度保護（不觸發）
  │
  └─ 有浮盈 → 時間止損不生效
```

所有參數基於 ATR 動態調整，不是固定值。

---

## 🖥️ Dashboard

即時監控網頁，深色主題，6 位像素角色各有個性動畫：

- 📊 **交易摘要** — 今日/本週損益 + 趨勢箭頭
- 📈 **持倉進度條** — 入場到止盈的視覺化位置
- 🎭 **AI 決策團隊** — 點擊角色可對話提問
- 📋 **共享布告欄** — 即時顯示各角色觀點
- ⚠️ **警告系統** — 異常自動置頂
- 📉 **損益曲線** — 最近 20 筆 sparkline

### 角色互動
每位角色可以直接對話：
- 點擊角色 → 跳動 + 氣泡框自我介紹
- 點「提問」→ 開啟對話框
- 角色根據自己的專業 + 即時系統數據回答

---

## 🔄 每日循環

```
每 10 分鐘：
  DataCollector → 9 策略投票 → Claude 分析 → Critic 把關 → 執行

每 3 分鐘：
  Position Manager → 評估持倉 → 讀布告欄 → 仲裁後決策

每 10 秒：
  Price Monitor → SL/TP/Breakeven/Lock2/Trail/Shadow 追蹤

每天 1 次：
  Daily Review（深度覆盤）→ Hypothesis Engine（產假設）
  → Update Deadzone（調封鎖）→ Evolver（全局評估）
```

---

## 🛡️ 風控

| 層級 | 門檻 | 動作 |
|---|---|---|
| 單筆止損 | ~2% | 平倉 + 冷卻 90min |
| 每日虧損 | 5% | 全天暫停 |
| 最大回撤 | 20% | 暫停至隔天 |
| 帳戶硬止損 | 25% | 永久停機 |
| Regime 禁止 | 極端恐慌禁做空 | 強制 hold |
| Conf Deadzone | 動態封鎖 | Shadow + 自動解封 |

---

## 🧬 技術棧

- **AI**：Claude Sonnet / Haiku（透過 CLI 呼叫）
- **語言**：Python 3.11+
- **交易所**：Binance Futures API
- **通知**：Discord Webhook（4 頻道分流）
- **監控**：自建 Web Dashboard（Flask + 靜態 HTML）
- **進程管理**：自建 Watchdog（File Lock 單一實例）

---

## 📝 開發筆記

這個系統從一個簡單的「Claude 分析市場 → 下單」開始，逐步演化成 6 角色協作系統。關鍵轉折點：

1. **單一 AI 的問題**：發現 Claude 太容易被單一指標誤導（一個 MACD cross 就平倉）
2. **加入 Critic**：從「建議」升級為「必要條件」，大幅減少衝動交易
3. **出場管理大修**：發現 80% 的虧損是「方向對但被止損掃掉」，重新設計 ATR 動態出場
4. **Shadow Trading**：封鎖表現差的區間，但用虛擬交易持續追蹤，避免永久錯過好機會
5. **Agent 布告欄**：讓角色之間能溝通，守護者知道分析師的觀點後不再亂平倉

每一步都是**被 bug 逼出來的設計**，不是事前規劃的架構。

---

## ⚠️ 免責聲明

本專案僅為技術概念展示，不構成投資建議。加密貨幣交易具有高風險，可能損失全部本金。

---

## 📄 License

MIT License

---

<div align="center">

*Built with Claude Code + 一堆被止損掃掉的教訓* 🏔️

</div>
