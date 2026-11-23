免膠繽紛聖誕花環 DIY 免費教學網頁｜芬妮手作

2026-11-23 起沿用芬妮 GA4（與雪人頁同一套）：`wreath_view`、`wreath_click_bNN`、`wreath_seen_bNN`。
36 個按鈕的固定識別、位置及目的地以 `tracking.json` 為準；新增或移動按鈕要同步更新，勿重新編號既有按鈕。
各平台入口連結（UTM）也在 `tracking.json` 的 `entry_links`。

上線前執行 `node --test tests/tracking.test.js`。本機部署 hook 以 `git config core.hooksPath .githooks` 啟用。
QA 用 `?fenny_qa=1&qa_run=<8位以內英數>`，事件進獨立 `wreath_qa_` 前綴，不送正式 page_view。

影片來源：Sally 手改定稿 `免膠繽紛聖誕花環_詳細教學_claude_v4.mp4`（5:46），轉 720×1280 後依草稿「步驟N｜…」字卡切 10 段（材料＋9 步），
每段開頭 1 秒為該步完成畫面（靜音）。
