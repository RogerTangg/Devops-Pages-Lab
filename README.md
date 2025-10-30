# DevOps A8: GitHub Pages & CI/CD Lab

這是DevOps 課程的第八次作業。

## 線上網站 (Live Site)

您可以在此查看自動部署的成果 (Live URL)：

**[https://RogerTangg.github.io/devops-pages-lab/](https://RogerTangg.github.io/devops-pages-lab/)**

---

## 運作原理 (How It Works)

本專案展示了一個自動化的 CI/CD 流程，用於更新並發布靜態網站。這滿足了作業的 O-Level 增強要求 (Documentation)。

**流程如下 (The flow is as follows):**

1.  **自動化工作流程 (Automation Workflow)**
    * 一個 GitHub Actions workflow (`.github/workflows/activity-log.yml`) 被設定為每日排程 (`schedule`) 或手動觸發 (`workflow_dispatch`) 運行。

2.  **內容抓取 (Content Fetching)**
    * Workflow 使用 `TheDanniCraft/activity-log` action 來抓取此儲存庫的最新公開活動。

3.  **自動提交 (Automated Commit)**
    * Action 將抓取到的活動日誌，自動寫入 (commit) 到本 `README.md` 檔案下方的 `Recent Activity` 區塊。

4.  **Jekyll 整合 (Jekyll Integration)**
    * 網站首頁 (`index.md`) 使用 Jekyll 語法 (`{% include_relative README.md %}`) 來動態包含 (include) `README.md` 的所有內容。

5.  **自動部署 (Automatic Deployment)**
    * 當 `README.md` 被機器人更新 (push) 時，會自動觸發 GitHub Pages 重新建置 (rebuild) 並部署網站，確保首頁始終顯示最新的活動日誌。

---

## 近期活動 (Recent Activity)
{% raw %}
<!--START_SECTION:activity-->
<!--END_SECTION:activity-->
{% endraw %}
