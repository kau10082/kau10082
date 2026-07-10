### 嗨，我是 Kao 👋

**不務正業的醫院工作者。** 白天在醫院上班，其餘時間都在玩各種 Claude skill 與自動化——從醫學資訊到天馬行空的點子，只要覺得有趣就想動手做做看。
*A hospital worker who can't quite stay in his lane — off the clock, tinkering with all sorts of Claude skills and automations, from medical-informatics tools to whatever wild idea sounds fun to try.*

---

### 🧭 我的 Claude skills & 工具 · My Claude skills & tools

<sub>每組由新到舊排列。狀態預設為 🟢 穩定運行；僅在 🟡 開發中／🔵 規劃中時額外標示。 · Newest first within each group. Assume 🟢 stable unless a 🟡 / 🔵 badge says otherwise.</sub>

#### 🩺 醫學文獻・簡報 · Medical literature & slides

- 🔎 **[slide-verify](https://github.com/kau10082/slide-verify)** 🆕<br>
  A one-stop skill for medical decks — verify → correct → reorder → split → plain-language rewrite — checking every citation and number against PubMed. It hunts the sneakiest distortions (real citations pinned to the wrong drug or a sister trial's numbers), flags what it can't verify instead of inventing it, and no matter how slides get reshuffled, every reference stays glued to the claim it supports.
  <details><summary>中文</summary>
  醫學簡報「驗證→勘誤→重排→拆頁→白話改寫」一條龍 skill，用 PubMed 逐條查證每個引用與數字。專抓「引用存在、卻掛錯藥或挑錯試驗數字」這類最隱蔽的失真，查不到就誠實標記，而且不管怎麼重排拆頁，reference 永遠跟著它支撐的內容走。
  </details>

- 📑 **[PPT-to-MD](https://github.com/kau10082/PPT-to-MD)** 🆕<br>
  Converts academic .pptx decks to Markdown exactly as they are — no guessing, no filler, honest blanks where recovery fails — even extracting the raw data behind native charts into clean tables. Pure Python standard library with zero install, and it happily eats the 25–50 MB files web converters reject.
  <details><summary>中文</summary>
  把學術與醫藥簡報（.pptx）原封不動轉成 Markdown：不猜測、不腦補、還原不了就誠實留白，連原生圖表的底層數據都能無損抽成表格。只用 Python 標準庫、零安裝，網頁轉檔工具拒收的 25–50MB 大檔也照吃。
  </details>

- 🎙️ **[transcript-fix](https://github.com/kau10082/transcript-fix)**<br>
  Not a speech-to-text tool — it rescues medical transcripts after transcription, fixing misheard drug names and numbers, a step the 600+ transcription projects on GitHub skip. Its unique combo: cross-checking multiple transcripts by majority vote, a self-growing Notion glossary, a focus on Traditional-Chinese-plus-English medical content — and it never makes anything up.
  <details><summary>中文</summary>
  不是語音轉文字，而是把轉完後藥名、數字被聽錯的醫學逐字稿「救回來」的修復工具——GitHub 上六百多個轉錄專案都不做這一步。獨家組合：多份逐字稿交叉比對、多數決收斂，搭配會自己長大的 Notion 詞庫，專攻繁中夾英的醫學內容，且絕不亂編。
  </details>

- 🔬 **[EBM_Framework](https://github.com/kau10082/EBM_Framework)**<br>
  Ask a clinical question in plain words and it runs the full EBM pipeline — find the research, verify each study is real, GRADE-appraise it, write the report — cross-checking every citation against Crossref/PubMed to kill hallucinations. Claude itself is the engine (no extra AI API key), and no report ships until every machine check passes.
  <details><summary>中文</summary>
  用白話問一個臨床問題，它就走完「找文獻→逐篇查證真偽→GRADE 評讀→產出報告」整條實證醫學流程，每篇引用都經 Crossref／PubMed 交叉查證去幻覺。以 Claude 本身為引擎、不需任何額外 AI API 金鑰，定稿前機器檢查全綠才放行。
  </details>

- 🩺 **[Pubmed_Bot](https://github.com/kau10082/Pubmed_Bot)**<br>
  A self-hosted PubMed alert bot: every day it finds new papers in your fields, writes AI summaries to your inbox, and files them into Zotero and Obsidian. A built-in journal-quality gate (SJR) keeps only the good papers so you're never flooded — running free on GitHub Actions, no subscription.
  <details><summary>中文</summary>
  自架的 PubMed 文獻追蹤機器人：每天自動找出你關注領域的新論文，AI 寫成中文摘要寄到信箱，並同步進 Zotero 與 Obsidian。內建期刊品質門檻（SJR）只留好論文、不被洪水淹沒，跑在免費的 GitHub Actions 上、零訂閱費。
  </details>

<sub>🔗 簡報工作流：`.pptx` →〔📑 PPT-to-MD〕→ 文字 →〔🔎 slide-verify〕→ 查證・重排。 · Deck workflow: .pptx →〔PPT-to-MD〕→ text →〔slide-verify〕→ verify & reorder.</sub>

#### 🧠 生產力・記憶 · Productivity & memory

- 📝 **[Note_Claude](https://github.com/kau10082/Note_Claude)**<br>
  A `/note-claud` command that archives note-worthy parts of your Claude chats into Google Drive / Obsidian word-for-word — it only moves, never summarizes or rewrites. It writes native `.md` files that slot straight into your existing vault, and skips (and warns about) anything private.
  <details><summary>中文</summary>
  一個 <code>/note-claud</code> 指令，把 Claude 對話中值得留下的段落「原封不動」存進 Google Drive／Obsidian——只搬運、不摘要、不改寫。直接產出 Obsidian 看得懂的 .md 檔融入你原本的筆記庫，遇到個資還會整段跳過並主動提醒。
  </details>

- 🧠 **[Project_Memory](https://github.com/kau10082/Project_Memory)**<br>
  Gives Claude a long-term memory: project progress and pitfalls are stored in your own Notion, and one `/load` in a fresh chat brings it all back — no re-explaining. claude.ai, Cowork, and Claude Code share the same memory, and the data lives in your Notion, fully under your control.
  <details><summary>中文</summary>
  讓 Claude 擁有長期記憶：專案進度、踩過的雷都存進你自己的 Notion，開新對話一句 <code>/load</code> 就全部叫回來，不必重複交代背景。網頁版、Cowork、Claude Code 共用同一套記憶，資料放在你的 Notion、完全由你掌握。
  </details>

#### 📊 監控・理財 · Monitoring & finance

- 📡 **[MOPS_Radar](https://github.com/kau10082/MOPS_Radar)**<br>
  A zero-server Taiwan-stock monitoring bot: every trading day it gathers major announcements, closing quotes, institutional buy/sell, shareholding distribution, and clinical-trial updates into a single Telegram message. It runs on GitHub Actions' free tier with a stateless, database-free design — set it up once and forget it.
  <details><summary>中文</summary>
  免伺服器的台股監控機器人：每個交易日自動彙整重大訊息、收盤行情、三大法人買賣超、集保股權分散與臨床試驗動態，濃縮成一則 Telegram 訊息。跑在 GitHub Actions 免費額度上、無資料庫的無狀態設計——設好一次就能忘記它。
  </details>

- 💳 **[Card_Radar](https://github.com/kau10082/Card_Radar)**<br>
  Which card should you swipe? Instead of a do-everything comparison app, it focuses on just the cards in your wallet and ranks them at the moment of payment by the actual cash you'd get back — never fooled by flashy rates or bonuses from wallets you don't use. Your card list and spending habits stay local, never uploaded.
  <details><summary>中文</summary>
  這筆該刷哪張卡？它不做大而全的比價 App，只針對你手上的卡，在付錢當下即時算出「實際拿到多少錢」來排名——不被漂亮的回饋率、也不被你根本沒在用的支付加碼騙。卡片清單與消費習慣全留在本機，絕不上傳。
  </details>

#### 🎮 其他・玩票 · Fun & misc

- 🎮 **[Game_ER_Night](https://github.com/kau10082/Game_ER_Night)**<br>
  A Taiwan-flavored, single-player ER night-shift text sim: survive 7 PM to 7 AM through hundreds of situation cards drawn from the real healthcare frontline — insurance claw-backs, entitled patients, political favors, litigious families — where doing the right thing goes unrewarded. Pure HTML/CSS/JS with zero dependencies and zero build: [just open the URL and play](https://kau10082.github.io/Game_ER_Night/).
  <details><summary>中文</summary>
  台灣特供的單人急診夜班文字模擬：從晚上 7 點撐到早上 7 點，上百張取材自醫療現場的情境卡，用黑色幽默演出核刪、鯛民、議員關說與告你的家屬——做對的事不會被獎勵。純 HTML/CSS/JS、零相依零建置，<a href="https://kau10082.github.io/Game_ER_Night/">打開網址就能玩</a>。
  </details>

<sub>🆕 最新加入 · Recently added　｜　狀態 Status：🟢 穩定運行 Stable · 🟡 開發中 In progress · 🔵 規劃中 Planned</sub>
