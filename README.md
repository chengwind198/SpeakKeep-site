# appsite

个人 App 的 GitHub Pages 站点：托管各应用的支持页、隐私政策页与使用条款页（英文 + 简体中文）。

| 应用 | 首页 | 支持 | 隐私政策 |
|---|---|---|---|
| SpeakKeep | `https://chengwind198.github.io/appsite/speakkeep/` | `https://chengwind198.github.io/appsite/speakkeep/support/` | `https://chengwind198.github.io/appsite/speakkeep/privacy/` |
| NovaPlayer | `https://chengwind198.github.io/appsite/novaplayer/` | `https://chengwind198.github.io/appsite/novaplayer/support/` | `https://chengwind198.github.io/appsite/novaplayer/privacy/` |

- 站点总览页：`https://chengwind198.github.io/appsite/`
- 各应用的文件分别放在对应目录下：`speakkeep/`、`novaplayer/`

## 启用 GitHub Pages（一次性）

仓库 **Settings → Pages → Build and deployment**：

- Source：**Deploy from a branch**
- Branch：**main** / **/ (root)**
- 保存后等 1–2 分钟即可访问。

## 更新方式

各应用的内容源在对应 App 仓库的 `site/`。改完后同步到这里：

```bash
# SpeakKeep
cp -R ../SpeakKeep/site/{index.html,assets.css,support,privacy} speakkeep/

# NovaPlayer
cp -R ../NovaPlayer/site/{index.html,assets.css,support,privacy,terms} novaplayer/

git add -A && git commit -m "sync site" && git push
```
