# ECUST课程分享仓库网站

这是一个基于GitHub Pages的华东理工大学课程资源分享网站，提供了友好的Web界面来浏览和下载课程资源。

## 功能特点

- 📚 提供完整的课程资源目录浏览
- 🔍 支持目录树形结构展示
- 📝 自动渲染并展示README文件内容
- 🔄 支持多个下载源切换(GitHub/Gitcode/CNB/Alist)
- 🌐 基于GitHub Pages的免费托管
- 🚀 无需维护和更新，自动调用API获取最新内容

## 技术实现

### 基础架构
- 托管平台: GitHub Pages
- 前端技术: 纯静态HTML/CSS/JavaScript
- API支持: CNB API / GitHub API (可切换)

### 两个版本
1. **CNB API版本** (index.html)
   - 使用CNB的API获取仓库内容
   - 通过CDN代理解决CORS限制 (cnbapi.bestzyq.cn)
   - 使用Alist的API实现搜索功能（alist.ecustvr.top）
   - 更稳定的国内访问体验

2. **GitHub API版本** (github.html)
   - 直接使用GitHub API获取仓库内容
   - 无需额外的CDN代理
   - 可能存在访问限制和连接问题

## 使用说明

### 访问网站
1. 主域名: [https://ecust-courseshare.github.io/](https://ecust-courseshare.github.io/)
2. 备用域名: [https://ecust-courseshare.ecustvr.top/](https://ecust-courseshare.ecustvr.top/) (解决移动网络访问问题)

### 浏览文件
1. 点击文件夹图标 📁 可以展开/折叠目录
2. 点击文件名可以查看文件内容
3. 每个文件都提供多个下载源供选择

### 下载源说明
- GitHub源：直接从GitHub仓库下载
- Gitcode源：使用Gitcode镜像下载
- CNB源：使用CNB平台下载
- Alist源：使用Alist服务器下载

## 已知问题

### CNB API版本:
- 需要通过CDN解决CORS限制
- README.md显示依赖cnb.ecustvr.top
- 需要定期更新证书

### GitHub API版本:
- 可能存在API访问限制
- 国内网络环境下可能连接不稳定

## 项目优势

- 🆓 完全免费的域名和托管服务
- 🔧 无需维护和手动更新
- 🔄 支持自定义下载源
- 📦 避免使用GitHub Actions（因仓库体积较大）

## 相关链接

- [项目仓库](https://github.com/ecust-CourseShare/ecust-courseshare.github.io)
- [课程资源仓库](https://github.com/tianyilt/ecust-CourseShare)
- [项目需求来源](https://github.com/tianyilt/ecust-CourseShare/issues/202)

## 贡献指南

如果你想为这个项目做出贡献，欢迎：
1. 提交Issue报告问题或建议新功能
2. 提交Pull Request改进代码
3. 帮助完善文档

## 开源协议

本项目采用MIT协议开源。
