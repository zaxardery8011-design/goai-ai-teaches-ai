# 用 AI 教導 AI

我們不是把答案餵給 AI。我們把「怎麼做、怎麼驗、踩過什麼坑」寫成 AI 讀得懂的檔，讓下一輪的 AI 自己學會。

## 一分鐘看懂

整包都是寫給 AI 讀的說明檔，**沒有程式**。帶走的是資料夾，不是一段提示詞。

四個技能，各舉一個用法：

| 技能 | 丟什麼進去 | 拿回什麼 |
|---|---|---|
| [yt-digest](skills/yt-digest/SKILL.md) | 一支 40 分鐘的工具教學網址 | 一頁：主旨、4～6 個重點、片中的工具與數字、一句洞見。缺任何一區就算失敗 |
| [copywriting-formula](skills/copywriting-formula/SKILL.md) | 「幫我寫一則介紹我自動化的貼文」 | 先套留帳體四段，第四段一定交代「怎麼知道它真的成了」，再挑 PAS／故事優先／迷思破解其中一套節奏 |
| [claim-spotcheck](skills/claim-spotcheck/SKILL.md) | 別的 AI 交回來的 repo 清單、星數、「查無」 | 逐筆打 API 驗。我們實跑過：9 個 repo 有 4 個 404；號稱 180 星，實測 2 星 |
| [skill-maker](skills/skill-maker/SKILL.md) | 一個你已經跑順的流程，例如會議錄音整理成紀要 | 一份 `SKILL.md`，下次換一個 AI 讀檔就會做 |

四個剛好一圈：skill-maker 負責產技能，claim-spotcheck 負責擋 AI 亂給來源，另外兩個一個吸收、一個輸出。
## 能做到什麼

| 你想做的 | 去哪 |
|---|---|
| 讓 AI 開瀏覽器：查資料、填表、抓網頁、批次整理、巡平台整理留言 | [browser-cdp](browser-cdp/README.md) |
| 一支影片變成繁中 digest | [skills/yt-digest](skills/yt-digest/SKILL.md) |
| 對外文案：留帳體＋公式庫＋誠實鐵律 | [skills/copywriting-formula](skills/copywriting-formula/SKILL.md) |
| 外部回件裡的網址、星數、否定斷言，依類型抽驗 | [skills/claim-spotcheck](skills/claim-spotcheck/SKILL.md) |
| 把你已經跑過的流程，寫成下一輪會照做的技能包 | [skills/skill-maker](skills/skill-maker/SKILL.md) |
| 丟一個連結，AI 幫你看懂 | [link-to-insight](link-to-insight/README.md) |
| 蒸餾自己的聲音：音色、口吻 | [voice-distill](voice-distill/README.md) |
| 用 AI 教 AI 的五條方法 | [lessons](lessons/README.md) |

巡平台整理留言這一項裡面包含海巡：沿關鍵字把留言收成一份，人決定回不回。不另開資料夾。

## 怎麼整合

每件都是一個資料夾。裡面有步驟、替代工具、驗收、紅線。AI 從 [START_HERE.md](START_HERE.md) 進來，先問你要做哪一件，再只讀那一夾。沒點名的先別讀。

| 資料夾 | 帶走什麼 |
|---|---|
| [START_HERE.md](START_HERE.md) | 給 AI 的入口。人類也可以先看這份。 |
| [browser-cdp](browser-cdp/README.md) | 用你看得到的瀏覽器查資料、填表、抓網頁、批次整理、巡留言。 |
| [skills/yt-digest](skills/yt-digest/SKILL.md) | 一支影片變成繁中 digest。本地轉錄優先。 |
| [skills/copywriting-formula](skills/copywriting-formula/SKILL.md) | 對外文案：留帳體＋公式庫＋誠實鐵律。 |
| [skills/claim-spotcheck](skills/claim-spotcheck/SKILL.md) | 外部 AI 回件裡的網址、星數、否定斷言，依類型抽驗。 |
| [skills/skill-maker](skills/skill-maker/SKILL.md) | 把你已經跑過的流程，寫成下一輪 AI 會照做的技能包。 |
| [link-to-insight](link-to-insight/README.md) | 丟一個連結，AI 幫你看懂。公開頁、要登入的頁、影片、長文。 |
| [voice-distill](voice-distill/README.md) | 蒸餾自己的聲音。兩條線：音色、口吻。含難度與三個坑。 |
| [lessons](lessons/README.md) | 用 AI 教 AI 的五條方法，每條附一個去識別的實例。 |
| [ideas](ideas/README.md) | 別人投稿的應用點子。收錄由維護者決定。 |
| [CONTRIBUTING.md](CONTRIBUTING.md) | 用 issue 或 PR 投稿的方式。 |

這份跟「送一則提示詞」差在哪：帶走的是資料夾。提示詞用完就沒了；檔可以改、可以傳、可以下一輪接著用。

丟進去之後：AI 問你要做哪一件時，回一件就好。做完看該件的驗收。沒過就還在做，不要收工。環境裡沒有某項工具，用該件寫的替代，不要停在缺工具。

## 怎麼開始

把這個 repo 丟給你的 AI，說「照 START_HERE 做」。

## 想再往下走

這包是教材。同一套方法，我們另外拆成幾個可以單獨拿的開源：

| repo | 管什麼 |
|---|---|
| [soplint](https://github.com/zaxardery8011-design/soplint) | 檢查你給 AI 定的規矩，不是檢查程式碼 |
| [execution-proofs](https://github.com/zaxardery8011-design/execution-proofs) | AI 說「做完了」，去看檔案是不是真的在、是不是新的 |
| [aiwff-checkup-public](https://github.com/zaxardery8011-design/aiwff-checkup-public) | 健檢你跟你的 AI 走到哪一關（測試版，會誤判） |
| [line-persona](https://github.com/zaxardery8011-design/line-persona) | 想讓 AI 在 LINE 上回話，從這裡開始 |
授權：MIT，見 [LICENSE](LICENSE)。
