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
1. 📝 Committed to [RogerTangg/Devops-Pages-Lab](https://github.com/RogerTangg/Devops-Pages-Lab/commit/92c913ac48ea7917e5884844c145868d1ab62a6f)
2. 📝 Committed to [RogerTangg/Devops-Pages-Lab](https://github.com/RogerTangg/Devops-Pages-Lab/commit/64077e6371451de0194bf333f8435890568a8bf4)
3. 📝 Committed to [RogerTangg/Devops-Pages-Lab](https://github.com/RogerTangg/Devops-Pages-Lab/commit/d775650c0a1c7d4561c31bdc32886d362acfd5cf)
4. 📝 Committed to [RogerTangg/Devops-Pages-Lab](https://github.com/RogerTangg/Devops-Pages-Lab/commit/14f6835fd2703a743cf7db64c07fcf9cb312e728)
5. 📝 Committed to [RogerTangg/Devops-Pages-Lab](https://github.com/RogerTangg/Devops-Pages-Lab/commit/284a8c5d203e45374c6c9d731f7b2274eec2a551)
<!--END_SECTION:activity-->
