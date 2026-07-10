### 嗨，我是 Kao 👋

**不務正業的醫院工作者。** 白天在醫院上班，其餘時間都在玩各種 Claude skill 與自動化——從醫學資訊到天馬行空的點子，只要覺得有趣就想動手做做看。
*A hospital worker who can't quite stay in his lane — off the clock, tinkering with all sorts of Claude skills and automations, from medical-informatics tools to whatever wild idea sounds fun to try.*

---

### 🧭 我的 Claude skills & 工具 · My Claude skills & tools

<sub>每組由新到舊排列。狀態預設為 🟢 穩定運行；僅在 🟡 開發中／🔵 規劃中時額外標示。 · Newest first within each group. Assume 🟢 stable unless a 🟡 / 🔵 badge says otherwise.</sub>

#### 🩺 醫學文獻・簡報 · Medical literature & slides

- 🔎 **[slide-verify](https://github.com/kau10082/slide-verify)** 🆕<br>
  把已是文字的醫學簡報丟給它，用 PubMed 逐條查證每個引用與數字，專抓最隱蔽的錯——引用都在、卻掛錯藥或挑錯試驗數字；查不到就誠實標記、絕不捏造。接著勘誤、重排投影片、把過載頁拆開，還能選擇改寫成白話，而且 reference 全程綁著它支撐的內容不脫鉤。PPT-to-MD 的下游好搭檔。
  <details><summary>English</summary>
  <i>Feed it the text of a medical deck and it fact-checks every citation and number against PubMed, catching the sneakiest errors — real papers pinned to the wrong drug, numbers cherry-picked from a sister trial — and flags anything unverifiable instead of inventing it. Then it corrects, reorders, splits overloaded slides, and can rewrite in plain language, with every reference staying glued to the claim it supports. A natural downstream companion to PPT-to-MD.</i>
  </details>

- 📑 **[PPT-to-MD](https://github.com/kau10082/PPT-to-MD)** 🆕<br>
  把學術與醫藥簡報（.pptx）原封不動轉成 Markdown：簡報寫什麼就抄什麼，不猜測、不腦補、不改寫，還原不了就誠實留白。連圖表底層的數據都能無損挖出成表格，並順手清掉頁碼、制式引註等雜訊。零安裝、只用 Python 標準庫，網頁工具吞不下的 25–50MB 大檔也照吃。
  <details><summary>English</summary>
  <i>Converts academic and medical .pptx decks into Markdown exactly as they are — copying only what the deck says (no guessing, no filler, honest blanks where recovery fails), losslessly extracting the data hidden inside charts into clean tables, and stripping page numbers and boilerplate noise. Zero install (Python standard library only), and it handles the 25–50 MB files web converters reject.</i>
  </details>

- 🎙️ **[transcript-fix](https://github.com/kau10082/transcript-fix)**<br>
  醫學演講、會議的語音逐字稿常把藥名、數據聽錯。它幫你校稿、重建語意：多份逐字稿交叉比對、絕不憑空捏造，還搭配一個會自動記下易混淆字詞、愈用愈準的 Notion 詞庫。
  <details><summary>English</summary>
  <i>Medical talk and meeting transcripts often mishear drug names and numbers. This skill proofreads and rebuilds the meaning — cross-checking multiple transcripts, never fabricating, backed by a self-growing Notion glossary that learns confusing terms as it goes.</i>
  </details>

- 🔬 **[EBM_Framework](https://github.com/kau10082/EBM_Framework)**<br>
  用白話問一個臨床問題，它就幫你找齊文獻、逐篇查證去幻覺、做 GRADE 評讀，再整理成報告。
  <details><summary>English</summary>
  <i>Ask a clinical question and it finds, verifies, and GRADE-appraises the evidence, then writes a report.</i>
  </details>

- 🩺 **[Pubmed_Bot](https://github.com/kau10082/Pubmed_Bot)**<br>
  每天自動巡 PubMed，挑出你關注領域的好論文、寫成中文摘要，送進 Zotero、信箱與 Obsidian。
  <details><summary>English</summary>
  <i>Sweeps PubMed daily and delivers AI-summarized papers to Zotero, your inbox, and Obsidian.</i>
  </details>

<sub>🔗 簡報工作流：`.pptx` →〔📑 PPT-to-MD〕→ 文字 →〔🔎 slide-verify〕→ 查證・重排。 · Deck workflow: .pptx →〔PPT-to-MD〕→ text →〔slide-verify〕→ verify & reorder.</sub>

#### 🧠 生產力・記憶 · Productivity & memory

- 📝 **[Note_Claude](https://github.com/kau10082/Note_Claude)**<br>
  一個 `/note-claud` 指令，把對話裡值得留下的主題原文歸檔進 Google Drive，日後再整理。
  <details><summary>English</summary>
  <i>A <code>/note-claud</code> command that files note-worthy conversation topics verbatim into Google Drive.</i>
  </details>

- 🧠 **[Project_Memory](https://github.com/kau10082/Project_Memory)**<br>
  一個讓 Claude「記得住」的 skill：把 Notion 當成跨對話的長期記憶庫，記下專案進度、踩過的雷、做到哪，下一個對話甚至換裝置都能無縫接續，不必再從頭交代背景。
  <details><summary>English</summary>
  <i>A skill that gives Claude lasting memory — it uses Notion as a cross-conversation knowledge base, recording your progress, pitfalls, and where you left off, so the next chat picks up right where you stopped.</i>
  </details>

#### 📊 監控・理財 · Monitoring & finance

- 📡 **[MOPS_Radar](https://github.com/kau10082/MOPS_Radar)**<br>
  免伺服器的台股雷達：靠 GitHub Actions 每天自動巡 MOPS 重大訊息、收盤價、法人籌碼，還有 ClinicalTrials.gov 的臨床試驗更新，整理成摘要推播到 Telegram。
  <details><summary>English</summary>
  <i>A zero-server Taiwan-stock radar: GitHub Actions sweeps MOPS announcements, closing prices, institutional trades, and ClinicalTrials.gov updates daily, then pushes a digest to Telegram.</i>
  </details>

- 💳 **[Card_Radar](https://github.com/kau10082/Card_Radar)**<br>
  錢包裡一堆卡，這筆該刷哪張？它把你的 Notion 當成個人信用卡資料庫，存放各卡的回饋規則，再依「實際拿到多少錢」而非帳面利率，即時挑出當下回饋最高的那張。用 `/card 全聯怎麼付` 這樣問就行。
  <details><summary>English</summary>
  <i>With a wallet full of cards, which one wins here? It uses your Notion as a personal credit-card database of reward rules, then ranks by the cash you'd actually earn — not the headline rate — to pick the best card for the purchase in front of you.</i>
  </details>

#### 🎮 其他・玩票 · Fun & misc

- 🎮 **[Game_ER_Night](https://github.com/kau10082/Game_ER_Night)**<br>
  台灣特供版的單人急診夜班模擬遊戲：從 19:00 撐到隔天 07:00，真正弄垮你的不是病人，而是核刪、鯛民、議員、長官 VIP、沒病房，還有動不動就告你的家屬——做對的事不會被獎勵。純前端、零相依，開瀏覽器就能玩。
  <details><summary>English</summary>
  <i>A darkly comic Taiwan-flavored solo ER night-shift sim: survive 19:00 to 07:00, where what really breaks you isn't the patients but insurance clawbacks, entitled complainers, meddling politicians, VIP bosses, no free beds, and families ready to sue — doing the right thing goes unrewarded. Pure front-end, zero dependencies, just open it in a browser.</i>
  </details>

<sub>🆕 最新加入 · Recently added　｜　狀態 Status：🟢 穩定運行 Stable · 🟡 開發中 In progress · 🔵 規劃中 Planned</sub>
