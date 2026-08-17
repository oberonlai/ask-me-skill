# ask-me — 個人品牌網站需求訪談 Skill

一個 Claude Code Skill，用「一問一答」的訪談方式，把你腦中模糊的想法變成 AI 可以直接拿去做網站的結構化文件。訪談結束後會自動產出 `website-brief.md`（需求文件）與 `CLAUDE.md`（後續做網站的專案設定）。

適合：做個人品牌網站、履歷網站、作品集網站，但還沒想清楚自己要什麼的人。

## 安裝方式

### 方法一：下載檔案手動安裝

1. 下載本 repo 的 `SKILL.md`。
2. 放到家目錄底下的這個路徑（資料夾不存在就自己建立）：

   ```
   ~/.claude/skills/ask-me/SKILL.md
   ```

### 方法二：讓 Claude Code 幫你裝

在專案資料夾啟動 `claude`，貼上這段提示詞：

```
請下載這個網址的內容，存成 ~/.claude/skills/ask-me/SKILL.md
（資料夾不存在就建立），完成後列出檔案清單，用繁體中文說明。
網址：https://raw.githubusercontent.com/oberonlai/ask-me-skill/main/SKILL.md
```

## 開始訪談

1. 在桌面建一個資料夾當網站專案，例如 `my-site`。
2. 終端機 `cd` 進去後輸入 `claude`。
3. 直接說「幫我做個人網站」或「使用 ask-me」即可啟動訪談。
4. 大部分題目會給選項，用點的就好；約 14 題、10 分鐘完成。

## 產出

訪談完成後，會在**目前的專案資料夾**建立兩個檔案：

- `website-brief.md` — 完整需求文件，可自行檢查、補充。
- `CLAUDE.md` — 後續做網站時 AI 要遵守的專案設定。

> ⚠️ 兩個檔案都會建立在你的專案資料夾，不會動到全域的 `~/.claude/CLAUDE.md`。
> 建立完成後請**重開一次 Claude Code**，新的 `CLAUDE.md` 才會被載入。
