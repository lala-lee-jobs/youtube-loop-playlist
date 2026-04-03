# haru-abc

YouTube 清單循環播放器（可儲存/載入清單、匯入/匯出 txt）。

## 部署到 GitHub Pages

### 1) 建立 GitHub Repo 並推上去

先在 GitHub 建立一個空 repo（例如 `haru-abc`），然後在本機執行：

```bash
git remote add origin https://github.com/<你的帳號>/<你的repo>.git
git add .
git commit -m "chore: setup github pages deploy"
git push -u origin main
```

如果你使用 SSH，remote 可改成：

```bash
git remote add origin git@github.com:<你的帳號>/<你的repo>.git
```

### 2) 開啟 GitHub Pages

1. 進入 GitHub repo 的 `Settings` -> `Pages`
2. `Build and deployment` 的 `Source` 選擇 `GitHub Actions`

### 3) 等待自動部署完成

本專案已包含 GitHub Actions workflow（`.github/workflows/pages.yml`），push 到 `main` 後會自動部署。

部署成功後網址通常會是：

`https://<你的帳號>.github.io/<你的repo>/`
