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
1. 🗑️ Deleted a branch `004-Add-Features` in [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version)
2. 📝 Committed to [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version/commit/42f0b91b8b18493c5ab9161e71767473b3b4093e)
3. 📝 Committed to [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version/commit/2f57b99837c9b632a23ec8f5408fab8d90645473)
4. 📝 Committed to [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version/commit/767665bf74e6ae74673e3f44dd5e0889bd913de9)
5. 📝 Committed to [RogerTangg/Virtual-Coach-App-New_Version](https://github.com/RogerTangg/Virtual-Coach-App-New_Version/commit/4ed74c1db8060a495d16fdbf8f982af5994f619d)
<!--END_SECTION:activity-->
