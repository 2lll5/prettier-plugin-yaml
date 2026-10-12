# Agent Instructions

## Google Drive Build 交付規範（所有 Agent 必須遵守）
- GitHub 專案 `prettier-plugin-yaml` 的 Build 專用 Google Drive：`AI Project/prettier-plugin-yaml/`（AI Project folder ID `1Yhfro6Ss5TSCXCVIZIHEu5h7V1gL8b27`）；專案資料夾與 Repo 名必須完全相同，不在 AI Project 頂層散放 ZIP。
- **根目錄只放最新完整且驗證成功的 Build（可有多平台）**：ZIP／執行包、SHA-256、各分割卷、必要還原／說明檔都一起交付；上傳後驗證名稱、父資料夾、大小及 checksum。缺少任何必要檔案（例如只有 checksum 沒有 ZIP）不可將新版標記最新版或移走之前的完整版本。
- **重大功能／架構／美術／平台差異**才建立 `vX.Y.Z-版本說明/`，一般舊版移到 `歷史封存/`，一律保留，避免每個小 Build 都增資料夾。
- 新開發推送 GitHub；昂貴 GitHub Actions 優先 `workflow_dispatch` 或正式 `release: published`，避免每次推 main 建置。完成時回報 Drive 資料夾、版本、檔案、驗證狀態；未真正編譯／測試／上傳不得假稱完成。
**English for agents:** Put newest verified complete build directly under `AI Project/prettier-plugin-yaml/`. Material milestone versions only in `vX.Y.Z-description/`; routine older builds in `歷史封存/`, never delete or promote partial upload.
