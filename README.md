# cloud-native-hw2

這是一個用於練習 GitHub Pull Request 和 GitHub Actions 的專案。

## 練習目的

本專案的目的是幫助開發者了解並練習如何使用 GitHub 提交 Pull Request (PR)，以及如何配置和使用 GitHub Actions 來自動化測試和構建流程。

### Pull Request (PR)

在這個專案中，你將學會如何創建和提交 Pull Request（PR）。PR 是協作開發中非常重要的工具，它允許開發者在提交代碼到主分支之前，進行代碼審查和討論。

- **創建 PR**: 當你在分支中完成某些修改後，創建 PR 來將這些修改合併到主分支。
- **代碼審查**: 提交 PR 後，其他開發者可以對代碼進行審查，提出修改建議，或者批准 PR 進行合併。
- **合併 PR**: 當 PR 被審查並通過後，它將被合併到主分支，並將這些變更應用到代碼庫中。

### GitHub Actions

GitHub Actions 是 GitHub 提供的 CI/CD（持續集成和持續部署）工具，允許開發者自動化各種工作流，比如測試、構建、部署等。

在這個專案中，我們使用 GitHub Actions 來執行自動化的測試和構建工作流。每次提交代碼或創建 PR 時，GitHub Actions 會自動觸發相應的工作流，保證代碼質量和功能正常。

#### 配置 GitHub Actions

1. **工作流文件**：在 `.github/workflows/` 目錄中，存放了所有的工作流配置文件。這些文件是 YAML 格式的，包含了工作流的具體配置，如測試、構建、部署等。
2. **CI/CD**：每次有代碼變更，GitHub Actions 會根據設定的觸發條件（例如 push 或 PR）自動執行相關的動作，如執行測試、構建應用或其他自定義操作。

#### 主要工作流步驟

- **測試**：每次 PR 被提交時，GitHub Actions 會自動運行測試，檢查代碼是否通過測試套件的檢查。
- **構建**：如果測試成功，GitHub Actions 會進一步構建應用，並進行靜態分析來確保代碼質量。

### 如何運行 GitHub Actions

1. **創建 PR 或推送代碼到分支**：
   當你推送代碼或創建 PR 時，GitHub Actions 會自動觸發工作流。
2. **查看工作流運行結果**：
   進入 GitHub 上的 `Actions` 標籤，你可以看到每個工作流的運行狀態，並查看詳細的運行日誌。

### 參考資源

- [GitHub Actions 官方文檔](https://docs.github.com/en/actions)
- [如何創建和提交 Pull Request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests)

