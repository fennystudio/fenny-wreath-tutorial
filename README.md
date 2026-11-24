免膠繽紛聖誕花環 DIY 免費教學網頁｜芬妮手作

2026-11-23 起沿用芬妮 GA4（與雪人頁同一套）：`wreath_view`、`wreath_click_bNN`、`wreath_seen_bNN`。
37 個按鈕的固定識別、位置及目的地以 `tracking.json` 為準；新增或移動按鈕要同步更新，勿重新編號既有按鈕。
連結只從自動私訊出去（ManyChat 的 IG／FB、Threads 活動私訊），`utm_source=ig|fb|threads&utm_medium=dm` 由 my-skills `fenny_shared/tutorial_links.py` 在送出平台確定時自動加；`entry_links` 只列 GA4 會看到的三種來源，不需手動貼。

上線前執行 `node --test tests/tracking.test.js`。本機部署 hook 以 `git config core.hooksPath .githooks` 啟用。
QA 用 `?fenny_qa=1&qa_run=<8位以內英數>`，事件進獨立 `wreath_qa_` 前綴，不送正式 page_view。

影片來源：Sally 手改定稿 `免膠繽紛聖誕花環_詳細教學_claude_v4.mp4`（5:46），轉 720×1280、補調色（原檔沒套草稿調色）後切成網頁 5 步；
片中燒入的「步驟N」字卡已逐格改成網頁步驟號 2～5，原第 2、6、7 步省略、8＋9 合併為第 5 步。每段開頭 1 秒為該步完成畫面（靜音）。
材料區只放材料表＋「材料表下」購買按鈕（`after_materials`），不放影片。
