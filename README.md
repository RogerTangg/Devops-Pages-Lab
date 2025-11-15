# DevOps A8: GitHub Pages & CI/CD 實驗室

## 線上網站 (Live Site)

您可以在此查看自動部署的成果 (Live URL)：

**[https:/rogertangg.github.io/devops-pages-lab/](https://rogertangg.github.io/devops-pages-lab/)**


---

## 運作原理 (How It Works)

本專案展示了一個自動化的 CI/CD 流程，用於更新並發布靜態網站。這滿足了作業的 O-Level 增強要求 (Documentation)。

**流程如下 (The flow is as follows):**

1.  **自動化工作流程 (Automation Workflow)**
    * 一個 GitHub Actions workflow (`.github/workflows/activity-log.yml`) 被設定為每日排程 (`schedule`) 或手動觸發 (`workflow_dispatch`) 運行。

2.  **內容抓取 (Content Fetching)**
    * Workflow 使用 `TheDanniCraft/activity-log` action 來抓取此儲存庫的最新公開活動。

3.  **自動提交 (Automated Commit)**
    * Action 將抓取到的活動日誌，自動寫入 (commit) 到本 `README.md` 檔案下方的 `最近活動` 區塊。

4.  **自動部署 (Automatic Deployment)**
    * 當 `README.md` 被機器人更新時，會自動觸發 GitHub Pages 重新建置 (rebuild)。
    * 內建的 `jekyll-readme-index` 插件會自動將此 `README.md` 檔案作為首頁內容，並套用 `_config.yml` 中指定的主題。

---

## 最近活動
<!--START_SECTION:activity-->
1. 📝 Committed to [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version/commit/f4d0ed946d8bbfff5779ef065b4783290aa92c6c)
2. 📥 Opened [PR #3](https://github.com/RogerTangg/Virtual-Coach-App-New_Version/pull/3) in [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version)
3. 📝 Committed to [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version/commit/e4857aaaa8d650f28552750d83d99d9386955403)
4. 🌍 Made repository [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version) public
5. 📝 Committed to [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version/commit/0c45fc5bd4a06580cb1aeae9d75ea61288f1fa6d)
<!--END_SECTION:activity-->
