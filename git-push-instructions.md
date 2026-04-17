# GitHub仓库创建和推送指南

## 步骤1：创建GitHub仓库

1. 登录你的GitHub账号：https://github.com
2. 点击页面右上角的 "+" 按钮，选择 "New repository"
3. 填写仓库信息：
   - **Repository name**: `FinderFavoritesSite`
   - **Description**: `FinderFavorites官方网站 - 提升你的Finder效率`（可选）
   - **Visibility**: 选择 `Public`（公开）
   - 不要勾选 "Add a README file"、"Add .gitignore" 或 "Choose a license"
4. 点击 "Create repository" 按钮

## 步骤2：推送本地代码到GitHub

仓库创建完成后，复制页面上的 "…or push an existing repository from the command line" 部分的命令，然后在终端中执行：

```bash
cd /Volumes/MACDATA/workspace/FinderFavorites/docs
git remote add origin https://github.com/code4happy/FinderFavoritesSite.git
git branch -M main
git push -u origin main
```

或者如果你使用SSH：

```bash
cd /Volumes/MACDATA/workspace/FinderFavorites/docs
git remote add origin git@github.com:code4happy/FinderFavoritesSite.git
git branch -M main
git push -u origin main
```

## 步骤3：启用GitHub Pages

1. 进入刚创建的 `FinderFavoritesSite` 仓库
2. 点击页面上方的 "Settings" 选项卡
3. 在左侧菜单中找到并点击 "Pages"
4. 在 "Source" 部分：
   - 选择 `main` 分支
   - 选择 `/root` 文件夹
   - 点击 "Save" 按钮
5. 等待几分钟，GitHub会自动部署你的网站
6. 网站将通过以下地址访问：
   `https://code4happy.github.io/FinderFavoritesSite/`

## 验证推送结果

推送完成后，你可以在GitHub仓库页面看到所有文件已成功上传。启用Pages后，访问上述URL即可看到你的网站。

## 后续更新

如果你需要更新网站内容，只需在本地修改文件后执行以下命令：

```bash
cd /Volumes/MACDATA/workspace/FinderFavorites/docs
git add .
git commit -m "更新网站内容：描述你做了什么修改"
git push origin main
```

更新后，GitHub Pages会自动重新部署网站，通常需要几分钟时间生效。
