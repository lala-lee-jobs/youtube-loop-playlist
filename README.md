# youtube-loop-playlist

可循環播放 YouTube 連結清單的網頁工具，支援清單儲存/載入與 TXT 匯入匯出。

## 功能

- 逐行貼上 YouTube 網址或影片 ID，依序播放
- 播放完自動跳下一首，並循環回第一首
- 可將目前清單儲存到瀏覽器（localStorage）
- 可從已儲存清單快速載入或刪除
- 支援 TXT 匯入與匯出

## 本機使用

直接用瀏覽器開啟 `index.html` 即可使用。

## 部署到 GitHub Pages

### 1) 建立 GitHub Repo 並推上去

先在 GitHub 建立空 repo（建議名稱：`youtube-loop-playlist`），再執行：

```bash
git remote add origin https://github.com/<你的帳號>/youtube-loop-playlist.git
git add .
git commit -m "chore: initialize project"
git push -u origin main
```

若你使用 SSH：

```bash
git remote add origin git@github.com:<你的帳號>/youtube-loop-playlist.git
```

### 2) 開啟 GitHub Pages

1. 到 repo 的 `Settings` -> `Pages`
2. 在 `Build and deployment` 將 `Source` 設為 `GitHub Actions`

### 3) 等待部署完成

本專案已包含 workflow：`.github/workflows/pages.yml`。  
每次 push 到 `main` 都會自動部署。

部署網址通常為：

`https://<你的帳號>.github.io/youtube-loop-playlist/`
