# SpeakKeep 站点

App Store Connect 使用的支持页与隐私政策页（英文 + 简体中文）。

| 页面 | 发布后地址 |
|---|---|
| 首页 | `https://chengwind198.github.io/SpeakKeep-site/` |
| 支持 | `https://chengwind198.github.io/SpeakKeep-site/support/` |
| 隐私政策 | `https://chengwind198.github.io/SpeakKeep-site/privacy/` |

## 启用 GitHub Pages（一次性）

仓库 **Settings → Pages → Build and deployment**：

- Source：**Deploy from a branch**
- Branch：**main** / **/ (root)**
- 保存后等 1–2 分钟即可访问。

## 更新方式

内容源在 App 仓库的 `site/`（`SpeakKeep/site`）。改完后同步到这里：

```bash
cp -R ../SpeakKeep/site/{index.html,assets.css,support,privacy} .
git add -A && git commit -m "sync site" && git push
```
