# Peicheng Wu — Academic Personal Website

Personal academic homepage, built as a plain static site (HTML + CSS, no build step) and hosted on **GitHub Pages**.

## 部署到 GitHub Pages（一次性设置）

1. 在 GitHub 上新建一个仓库，命名为 `<你的用户名>.github.io`（例如 `peichengwu.github.io`）。
   仓库名必须严格是这个格式，网站才会发布在根域名 `https://<你的用户名>.github.io`。
2. 在本目录下执行：

   ```powershell
   git init
   git add .
   git commit -m "Initial academic website"
   git branch -M main
   git remote add origin https://github.com/<你的用户名>/<你的用户名>.github.io.git
   git push -u origin main
   ```

3. 打开仓库的 **Settings → Pages**，确认 Source 为 `Deploy from a branch`，Branch 选 `main` / `(root)`，保存。
4. 一两分钟后访问 `https://<你的用户名>.github.io` 即可看到网站。

## 日常更新

- **添加论文**：编辑 `index.html` 中 `<!-- PUBLICATIONS -->` 区域，复制一个 `<li class="pub-item">` 块改内容即可。
- **更新照片**：把头像图片放到 `images/profile.jpg`（正方形裁剪效果最佳）。
- **改完后**：`git add . ; git commit -m "update" ; git push`，约 1 分钟后自动生效。

## 文件结构

```
index.html        — 整站内容（单页：About / Publications / Education / Contact）
css/style.css     — 样式（含深色模式、移动端适配）
images/           — 头像等图片
.nojekyll         — 告诉 GitHub Pages 跳过 Jekyll 构建，直接发布静态文件
```
