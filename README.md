# Yanting Yang 个人主页

纯静态网站：`index.html` + `style.css`，不需要任何构建工具，直接放到 GitHub Pages 就能用。

## 文件
- `index.html`：所有内容（简介、研究方向、工作经历、News、论文）
- `style.css`：样式，自动适配浅色 / 深色模式和手机
- `images/`：头像 `profile.jpg` 和论文配图
- `favicon.svg`：浏览器标签页图标
- `.nojekyll`：让 GitHub Pages 原样发布文件，不用 Jekyll 处理

## 常见修改
- **加一条 News**：在 `index.html` 的 `<ul class="news">` 最上面复制一行 `<li>`。旧的可以挪进 "Earlier news" 折叠区。
- **加一篇论文**：复制一个 `<article class="pub">...</article>` 块，改标题、作者、会议、链接。
- **换论文配图**：直接用同名文件替换 `images/` 里的图（如 `images/space.png`）。论文配图来自各论文的 teaser / Figure 1。
- **加 LinkedIn**：在 `index.html` 里搜 `YOUR-LINKEDIN-ID`，换成你的链接，再去掉那一段外面的 `<!--` 和 `-->`。
- **本地预览**：直接双击 `index.html` 用浏览器打开即可。

## 更新网站
这个文件夹已经连着 GitHub 仓库 `Yt2000/Yt2000.github.io` 的 `master` 分支。改完以后：

```bash
git add -A
git commit -m "Update homepage"
git push
```

推上去一两分钟后 https://yt2000.github.io/ 就会更新。旧网站还留在 git 历史里，需要时可以找回。

## 第一次开启 GitHub Pages（只需做一次）
GitHub 上打开仓库 → Settings → Pages → Build and deployment：
Source 选 **Deploy from a branch**，Branch 选 **master** / **(root)** → Save。
