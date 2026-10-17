# Build Server Docker 狀態報告:圖表與簡報

本資料夾與 `../deck/` 放的是「Build Server 容器化編譯環境」狀態報告的圖表與簡報。內容依報告整理,時程日期僅為示意(假設 2026-10-19 起算)。

## 原始檔(Figma)

| 內容 | 連結 |
|---|---|
| FigJam 圖表(4 張圖) | https://www.figma.com/board/HtUXm19VvZ52WzCEpp6fpQ |
| Figma Slides 簡報(9 頁) | https://www.figma.com/slides/YZiIaxwMBMORUnILBKfAgf |

這兩份是個人 Figma 檔,只有被分享的人才打得開。需要團隊共用時,請先在 Figma 內分享,或搬進團隊空間。

## 檔案對照

| Repo 檔案 | FigJam section |
|---|---|
| `diagrams/01_container_architecture.png` | 1. 容器化編譯環境架構 |
| `diagrams/02_deploy_flow.png` | 2. 部署到 Build Server 流程 |
| `diagrams/03_cicd_pipeline.png` | 3. 目標 CI/CD 流程與完成狀態 |
| `diagrams/04_cicd_timeline.png` | 4. CI/CD 時程 P0 到 P6 (預估) |

`deck/Build_Server_Docker_Status.pptx` 是可在 PowerPoint 編輯的版本,頁面順序與 Figma 簡報相同:

1. 標題
2. 一頁摘要
3. 容器化編譯環境架構
4. 部署到 Build Server 的流程
5. 目標 CI/CD 流程與完成狀態
6. 狀態檢查
7. CI/CD 時程
8. 在 Build Server 使用 LLM CLI 的評估
9. 需要主管決策或協助

pptx 是依同一份內容另外產生的,兩邊版面略有差異;改了其中一份,另一份不會自動同步。

## 更新方式

- **PNG:** 在 FigJam 選取對應的 section,用 Export 匯出 PNG,覆蓋本資料夾同名檔案。
- **簡報:** 在 Figma Slides 修改後,pptx 需要另外更新;可在 PowerPoint 直接改 pptx,或重新匯出。
- 圖 1 到 3 是流程圖,改文字或移動節點時連線會跟著走。圖 4 的時程是用形狀拼成,不是真正的甘特圖,改日期要手動調整色條。

## 內容限制

- 「已驗證」只指實際執行並看到結果的項目;時程與預期效益都是預估,不是承諾。
- 目前只在 WSL 模擬的 Ubuntu 22.04 驗證,尚未在實體 Build Server 執行。
