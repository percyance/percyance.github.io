# Peicheng Wu — Academic Personal Website

Personal academic homepage, built as a plain static site (HTML + CSS, no build step) and hosted on **GitHub Pages**.

- **线上地址**: <https://percyance.github.io>
- **仓库**: <https://github.com/percyance/percyance.github.io>（`main` 分支根目录直接发布）

## 日常更新

- **添加论文**：编辑 `index.html` 中 `<!-- PUBLICATIONS -->` 区域，复制一个 `<li class="pub-item">` 块改内容即可。
- **更新照片**：替换 `images/profile.jpg`（正方形裁剪效果最佳）。
- **开通 Google Scholar 后**：取消 `index.html` 头部链接区注释掉的 Google Scholar 链接，填入你的 user id。
- **改完后**：`git add . ; git commit -m "update" ; git push`，约 1 分钟后自动生效。

## 文件结构

```
index.html        — 整站内容（单页：About / Publications / Education / Contact）
css/style.css     — 样式（含深色模式、移动端适配）
images/           — 头像等图片
.nojekyll         — 告诉 GitHub Pages 跳过 Jekyll 构建，直接发布静态文件
```
