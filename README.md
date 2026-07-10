### 嗨，我是 Kao 👋

**不務正業的醫院工作者。** 白天在醫院上班，其餘時間都在玩各種 Claude skill 與自動化——從醫學資訊到天馬行空的點子，只要覺得有趣就想動手做做看。
*A hospital worker who can't quite stay in his lane — off the clock, tinkering with all sorts of Claude skills and automations, from medical-informatics tools to whatever wild idea sounds fun to try.*

---

### 🧭 我的 Claude skills & 工具 · My Claude skills & tools

<sub>每組由新到舊排列。狀態預設為 🟢 穩定運行；僅在 🟡 開發中／🔵 規劃中時額外標示。 · Newest first within each group. Assume 🟢 stable unless a 🟡 / 🔵 badge says otherwise.</sub>

#### 🩺 醫學文獻・簡報 · Medical literature & slides

- 🔎 **[slide-verify](https://github.com/kau10082/slide-verify)** 🆕<br>
  把醫學簡報的每個引用與數字丟到 PubMed 逐條查證，再自動勘誤、重排投影片。連「論文是真的、卻掛錯藥或挑錯數字」這種最隱蔽的錯都抓得到，查不到就誠實標記、絕不捏造。<br>
  *Fact-checks every citation and number in a medical deck against PubMed, then corrects and reorders the slides. It catches even the sneakiest errors — real papers pinned to the wrong claim — and flags what it can't verify instead of inventing it.*

- 📑 **[PPT-to-MD](https://github.com/kau10082/PPT-to-MD)** 🆕<br>
  把學術與醫藥簡報（.pptx）原封不動轉成 Markdown：不猜測、不腦補，連圖表底層數據都能無損挖成表格。零安裝、只用 Python 標準庫，網頁工具吞不下的 25–50MB 大檔也照吃。<br>
  *Converts academic .pptx decks to Markdown exactly as written — no guessing, no filler — even extracting the raw data inside charts into clean tables. Zero install (pure Python standard library), and it handles the 25–50 MB files web converters reject.*

- 🎙️ **[transcript-fix](https://github.com/kau10082/transcript-fix)**<br>
  專治語音逐字稿聽錯藥名與數據：多份逐字稿交叉比對、重建語意、絕不憑空捏造。搭配會自動累積易混淆詞的 Notion 詞庫，愈用愈準。<br>
  *Proofreads medical transcripts where speech-to-text mishears drug names and numbers — cross-checking multiple transcripts, never fabricating. A self-growing Notion glossary makes it more accurate with every use.*

- 🔬 **[EBM_Framework](https://github.com/kau10082/EBM_Framework)**<br>
  用白話問一個臨床問題，它就找齊文獻、逐篇查證去幻覺、做 GRADE 評讀，再寫成報告。一條龍的實證醫學流程。<br>
  *Ask a clinical question in plain language and it finds, verifies, and GRADE-appraises the evidence, then writes the report — a full EBM pipeline with built-in hallucination checks.*

- 🩺 **[Pubmed_Bot](https://github.com/kau10082/Pubmed_Bot)**<br>
  每天自動巡 PubMed，把你關注領域的新論文寫成中文摘要，送進 Zotero、信箱與 Obsidian。設定一次，文獻自己送上門。<br>
  *Sweeps PubMed daily and delivers AI-summarized papers in your fields to Zotero, your inbox, and Obsidian. Set it up once and the literature comes to you.*

<sub>🔗 簡報工作流：`.pptx` →〔📑 PPT-to-MD〕→ 文字 →〔🔎 slide-verify〕→ 查證・重排。 · Deck workflow: .pptx →〔PPT-to-MD〕→ text →〔slide-verify〕→ verify & reorder.</sub>

#### 🧠 生產力・記憶 · Productivity & memory

- 📝 **[Note_Claude](https://github.com/kau10082/Note_Claude)**<br>
  一個 <code>/note-claud</code> 指令，把對話裡值得留下的主題原文歸檔進 Google Drive。先留存、後整理，好點子不再隨對話結束而消失。<br>
  *A `/note-claud` command that files note-worthy conversation topics verbatim into Google Drive. Capture now, organize later — good ideas no longer vanish when the chat ends.*

- 🧠 **[Project_Memory](https://github.com/kau10082/Project_Memory)**<br>
  用 Notion 當 Claude 的跨對話長期記憶，記下專案進度、踩過的雷與做到哪。下個對話、甚至換裝置都能無縫接續，不必重講背景。<br>
  *Gives Claude lasting memory by using Notion as a cross-conversation knowledge base — progress, pitfalls, where you left off. The next chat picks up right where you stopped, even on another device.*

#### 📊 監控・理財 · Monitoring & finance

- 📡 **[MOPS_Radar](https://github.com/kau10082/MOPS_Radar)**<br>
  免伺服器的台股雷達：GitHub Actions 每天自動巡 MOPS 重大訊息、收盤價、法人籌碼與 ClinicalTrials.gov 更新，摘要直接推播到 Telegram。全程零成本運行。<br>
  *A zero-server Taiwan-stock radar: GitHub Actions sweeps MOPS announcements, closing prices, institutional flows, and ClinicalTrials.gov daily, then pushes a digest to Telegram — all for free.*

- 💳 **[Card_Radar](https://github.com/kau10082/Card_Radar)**<br>
  這筆該刷哪張卡？它把你的 Notion 當成個人信用卡回饋規則庫，依「實際拿到多少錢」而非帳面利率，即時挑出當下最划算的那張。<br>
  *Which card should you swipe? Using your own Notion as a database of reward rules, it ranks cards by the cash you'd actually earn — not the headline rate — and picks the winner for the purchase in front of you.*

#### 🎮 其他・玩票 · Fun & misc

- 🎮 **[Game_ER_Night](https://github.com/kau10082/Game_ER_Night)**<br>
  黑色幽默的台灣特供急診夜班模擬：從 19:00 撐到隔天 07:00，弄垮你的不是病人，而是核刪、鯛民、VIP 與動輒提告的家屬。純前端、零相依，開瀏覽器就能玩。<br>
  *A darkly comic, Taiwan-flavored ER night-shift sim: survive 19:00–07:00, where insurance clawbacks, VIPs, and litigious families break you before the patients do. Pure front-end, zero dependencies — just open it in a browser.*

<sub>🆕 最新加入 · Recently added　｜　狀態 Status：🟢 穩定運行 Stable · 🟡 開發中 In progress · 🔵 規劃中 Planned</sub>
