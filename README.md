# 用 AI 教導 AI

我們不是把答案餵給 AI。我們把「怎麼做、怎麼驗、踩過什麼坑」寫成 AI 讀得懂的檔，讓下一輪的 AI 自己學會。

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

授權：MIT，見 [LICENSE](LICENSE)。
