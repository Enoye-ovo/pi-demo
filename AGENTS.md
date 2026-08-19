# pi-demo 部署指南

## 项目信息
- 目录：D:/pi-demo
- GitHub 仓库：Enoye-ovo/pi-demo
- 访问地址：https://enoye-ovo.github.io/pi-demo/ 或 https://www.enoye.cn
- 自定义域名：enoye.cn（阿里云 DNS → GitHub Pages）

## 部署流程
1. 修改 `index.html`（页面内容）
2. 执行以下命令提交并推送：
   ```bash
   cd D:/pi-demo && git add index.html && git commit -m "描述信息" && git push origin main
   ```
3. GitHub Actions 会自动部署到 GitHub Pages

## 注意事项
- Git 需要配置 safe.directory：`git config --global --add safe.directory D:/pi-demo`
- 推送后在 https://github.com/Enoye-ovo/pi-demo/actions 查看部署状态
- 也可用 API 查状态：`curl -s "https://api.github.com/repos/Enoye-ovo/pi-demo/actions/runs?per_page=1" | grep -E '"status"|"conclusion"'`
- CNAME 文件已配置自定义域名 enoye.cn，不要删除

## 历史版本
- 七夕星空版（当前）
- 七夕年轻风 Magoni 版
- 七夕古风版
- 待办清单 demo
