### 嗨，我是 Kao 👋

**不務正業的醫院工作者。** 白天在醫院上班，其餘時間都在玩各種 Claude skill 與自動化——從醫學資訊到天馬行空的點子，只要覺得有趣就想動手做做看。
*A hospital worker who can't quite stay in his lane — off the clock, tinkering with all sorts of Claude skills and automations, from medical-informatics tools to whatever wild idea sounds fun to try.*

---

### 🧭 我的 Claude skills & 工具 · My Claude skills & tools

#### 🩺 醫學文獻・簡報 · Medical literature & slides

- 🔤 **[pdf-text-recover](https://github.com/kau10082/pdf-text-recover)** 🆕<br>
  A pre-repair station for PDF text-extraction pipelines (e.g. PDF→Markdown): when extraction comes out garbled, it rebuilds the text layer deterministically from the font's own data — OCR only verifies, it never decides.<br>
  PDF 文字萃取管線（如 PDF→Markdown）的前置修復站：抽出亂碼時，從字型線索確定性修復文字層，OCR 只當驗證者。

- 📚 **[epub-extract](https://github.com/kau10082/epub-extract)**<br>
  A Claude skill for faithful, auditable whole-book extraction into knowledge-base-ready Markdown — not a summary. A standard-library verifier fails loudly the moment an image or chapter is silently dropped.<br>
  把整本電子書忠實萃取成知識庫可用的 Markdown 的 Claude 技能——不是摘要。內建純標準庫的機械對帳，一旦吞圖、掉章就大聲報錯，絕不安靜出錯。

- 🔎 **[slide-verify](https://github.com/kau10082/slide-verify)**<br>
  A Claude Skill that fact-checks medical slide decks against PubMed — verify → correct → reorder → split → plain-language rewrite. It catches real papers *cited wrongly*, not just fabricated ones, tracing every number back to the source to confirm the paper actually said it.<br>
  醫學簡報文獻查核一條龍 Claude Skill：驗證→勘誤→重排→拆頁→白話改寫。不只查文獻存不存在，更追進原文核對「這篇真文獻到底有沒有說過這個數字」，專抓真文獻被引錯的隱蔽失真。

- 📑 **[PPT-to-MD](https://github.com/kau10082/PPT-to-MD)**<br>
  A Claude skill that converts .pptx decks to Markdown exactly as they are — chart data extracted losslessly, speaker notes sorted, no AI guessing. Built for academic and medical slides.<br>
  把簡報原封不動轉成 Markdown 的 Claude skill：圖表數據無損還原、講者備註自動分類、純機械不腦補，專為學術醫藥簡報設計。

- 🎙️ **[transcript-fix](https://github.com/kau10082/transcript-fix)**<br>
  A Claude skill that proofreads and semantically reconstructs error-dense medical ASR transcripts — multi-transcript diff, never fabricates, powered by a self-growing Notion glossary that learns confusing terms automatically.<br>
  醫學語音逐字稿校稿與語意重建的 Claude skill：多稿交叉比對、絕不捏造，搭配「會自動記錄易混淆字詞、自我成長」的 Notion 詞庫。

- 🔬 **[EBM_Framework](https://github.com/kau10082/EBM_Framework)**<br>
  End-to-end evidence-based medicine, not just one slice: ask in plain language and it finds the studies, verifies each is real (Crossref/PubMed anti-hallucination plus word-for-word number checks), grades with GRADE, and writes the report. Claude is the engine — no extra AI API.<br>
  一句白話問題到報告一條龍：找文獻→逐篇查證去幻覺→GRADE 評讀→出報告。以 Claude 本身為引擎，不需額外 AI API。

- 🩺 **[Pubmed_Bot](https://github.com/kau10082/Pubmed_Bot)**<br>
  A daily PubMed literature-alert and monitoring bot: AI paper summaries delivered to your inbox, Zotero, and Obsidian. A free, self-hosted alternative to PubMed email alerts / RSS.<br>
  每天自動追蹤 PubMed 新論文、用 AI 產生中文摘要，一次送進 Email、Zotero 與 Obsidian——PubMed Email Alert／RSS 的免費自架替代方案。

#### 🧠 生產力・記憶 · Productivity & memory

- 📝 **[Note_Claude](https://github.com/kau10082/Note_Claude)**<br>
  A Claude Code skill that archives your Claude AI chats word-for-word into Obsidian / Google Drive — one command, saved by topic, no summaries or rewriting.<br>
  在 Claude 裡做筆記：一句指令把對話原文逐字歸檔進 Obsidian／Google Drive，依主題存放，不摘要、不改寫。

- 🧠 **[Project_Memory](https://github.com/kau10082/Project_Memory)**<br>
  A Claude skill that gives Claude long-term memory via Notion — reload any project and resume seamlessly across conversations.<br>
  讓 Claude 跨對話記得住的 skill：用 Notion 當長期記憶庫，開新對話也能無縫接續、把任何專案叫回來。

#### 📊 監控・理財 · Monitoring & finance

- 📡 **[MOPS_Radar](https://github.com/kau10082/MOPS_Radar)**<br>
  A zero-server Taiwan-stock bot on GitHub Actions — a daily Telegram digest of MOPS announcements, quotes, institutional trades, TDCC shareholding, and ClinicalTrials.gov updates.<br>
  免伺服器台股監控機器人：每日自動追蹤重大訊息、行情、三大法人、集保股權與臨床試驗，推播到 Telegram。

- 💳 **[Card_Radar](https://github.com/kau10082/Card_Radar)**<br>
  A Claude Skill that tells you which credit card to swipe before you pay — ranks by real cashback after monthly caps, counts only the cards and wallets you actually use, knows Taiwan's local exclusion rules, and keeps all data on your own machine.<br>
  付款前問一句就知道刷哪張卡最划算的 Claude Skill：只看你手上的卡、算扣掉上限後的實拿回饋、懂台灣在地排除規則、個資全留本機。

#### 🎮 其他・玩票 · Fun & misc

- 🎮 **[Game_ER_Night](https://github.com/kau10082/Game_ER_Night)**<br>
  A Taiwan-flavored, single-player ER night-shift sim: survive 19:00 to 07:00, where what really breaks you is insurance clawbacks, entitled complainers, politicians, VIP bosses, no free beds, and families ready to sue — doing the right thing goes unrewarded. Pure front-end, zero dependencies, [open it in a browser and play](https://kau10082.github.io/Game_ER_Night/).<br>
  台灣特供版的單人急診夜班模擬遊戲：19:00 撐到 07:00，真正弄垮你的是核刪、鯛民、議員、長官 VIP、沒病房和告你的家屬——做對的事不會被獎勵。純前端、零相依、開瀏覽器即玩。

<sub>🆕 最新加入 · Recently added</sub>
