# FinderFavorites GitHub Pages 网站

这是 FinderFavorites 的官方网站，通过 GitHub Pages 托管。

## 网站内容

- **功能介绍**：详细介绍 FinderFavorites 的各项功能
- **版本对比**：免费版和专业版的功能差异
- **了解升级**：为什么要升级到专业版

## 如何启用 GitHub Pages

1. 登录 GitHub，进入 FinderFavorites 仓库
2. 点击 "Settings"（设置）选项卡
3. 在左侧菜单中找到 "Pages" 选项
4. 在 "Source"（源）部分，选择 "main branch /docs folder"（main分支 /docs文件夹）
5. 点击 "Save"（保存）
6. 等待几分钟，网站将通过 `https://yourusername.github.io/FinderFavorites/` 访问

## 自定义域名（可选）

如果您想使用自定义域名：

1. 在域名服务商处添加一个 CNAME 记录，指向 `yourusername.github.io`
2. 在本目录下创建一个名为 `CNAME` 的文件，内容为您的自定义域名（例如：`www.finderfavorites.com`）
3. 提交并推送到 GitHub
4. 在 GitHub Pages 设置中启用自定义域名

## 网站维护

### 修改内容

直接编辑 `index.html` 文件即可修改网站内容。网站使用以下技术：

- HTML5
- Tailwind CSS（通过 CDN）
- Font Awesome 图标（通过 CDN）
- 原生 JavaScript

### 添加新页面

如果需要添加新页面，只需在 `docs` 目录下创建新的 HTML 文件，并更新导航链接。

## 本地预览

在本地预览网站，可以使用以下方法：

### 方法 1：使用 Python

```bash
# Python 2
python -m SimpleHTTPServer 8000

# Python 3
python3 -m http.server 8000
```

然后在浏览器中访问 `http://localhost:8000`

### 方法 2：使用 Node.js

```bash
npx serve .
```

然后在浏览器中访问显示的地址（通常是 `http://localhost:3000`）

### 方法 3：使用 VS Code 扩展

安装 "Live Server" 扩展，右键点击 `index.html` 文件，选择 "Open with Live Server"

## 技术支持

如果在使用 GitHub Pages 过程中遇到问题，请参考：
- [GitHub Pages 官方文档](https://docs.github.com/cn/pages)
- [GitHub Pages 故障排除](https://docs.github.com/cn/pages/troubleshooting)
