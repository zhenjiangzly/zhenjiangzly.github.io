# Andante · 个人主页

一个可直接打开和发布的静态个人网站。米白与墨绿配色，适配手机和电脑，正文为中文。没有安装或构建步骤，也没有付费托管、外部字体或脚本依赖。

## 你的入口

- GitHub 账号：`zhenjiangzly`
- 网站仓库：`zhenjiangzly.github.io`
- 网站地址：https://zhenjiangzly.github.io/
- 仓库地址：https://github.com/zhenjiangzly/zhenjiangzly.github.io

以上为本项目的目标地址；是否已上线，以 GitHub Pages 的发布状态和实际访问结果为准。

## 从零搭建的步骤

### 1. 准备账号

已有 GitHub 账号可以直接登录。没有账号时，在 https://github.com/signup 按提示注册并验证邮箱。你的当前连接账号已经是 `zhenjiangzly`，无需重新注册。

### 2. 建立网站仓库

登录后打开 https://github.com/new 。

1. Owner 选择自己的账号。
2. Repository name 填 `zhenjiangzly.github.io`。换一个账号时，必须改成该账号的 `用户名.github.io`。
3. Visibility 选 **Public**，使用免费 GitHub Pages。
4. 点击 **Create repository**。

Andante 是页面上的名字，仓库仍使用账号对应的名称。仓库可以理解为存放网站文件的文件夹。

### 3. 上传网站文件

在仓库中选择 **Add file → Upload files**。若仓库为空，点 **uploading an existing file**。

上传本文件夹里的 `index.html`、`styles.css`、`favicon.svg`、`.nojekyll` 和 `README.md`。文件应直接位于仓库根目录，不要把外层 `andante` 文件夹一起上传。页面入口一定要叫 `index.html`。

填写简短说明，例如 `Publish Andante homepage`，再点 **Commit changes**。

### 4. 开启 GitHub Pages

进入仓库 **Settings → Pages**：

1. 在 **Build and deployment** 中，Source 选 **Deploy from a branch**。
2. Branch 选 **main**；目录选 **/(root)**。
3. 点击 **Save**。
4. 保持 Custom domain 为空。

这里的 main 是网站文件所在的主分支；/(root) 表示从最外层目录发布。无需手动编写 GitHub Actions。

### 5. 检查上线结果

发布完成后，Settings → Pages 会显示网站链接，点 **Visit site**。

检查标题是否为 Andante，导航是否跳到对应章节，GitHub 入口是否正确。手机打开后，页面应为单列且没有横向滚动。首次发布或更新可能需要最多约 10 分钟。

## 本地预览

双击 `index.html` 即可在浏览器中预览。把浏览器窗口缩窄，可以查看手机版布局。

## 以后怎样修改

1. 打开仓库中的 `index.html`，点铅笔图标编辑。
2. 修改标题、介绍、兴趣描述或 GitHub 链接。保留文字周围的 HTML 标签。
3. 点 **Commit changes**。GitHub Pages 会重新发布。

常用位置：

| 想修改的内容 | 文件与位置 |
| --- | --- |
| 浏览器标题与搜索摘要 | `index.html` 顶部的 `title` 和 `description` |
| 主标题、简介和关于文字 | `index.html` 的 hero 与 about 区域 |
| 三个兴趣方向 | `index.html` 的 interests 区域 |
| GitHub 地址 | `index.html` 的 connect 区域 |
| 背景、文字与分隔线颜色 | `styles.css` 顶部的 `:root` |
| 页脚年份 | `index.html` 最后的 footer |

当前简介是依据兴趣写的可修改初稿，没有预设学历、职业、成绩或项目经历。

## 常见问题

- **看到 404**：先检查 Settings → Pages 是否保存了 main 与 /(root)，根目录是否有 `index.html`，然后等待首次部署完成。
- **页面没有样式**：检查 `styles.css` 是否与 `index.html` 在同一层，文件名大小写是否一致。
- **更新没有出现**：等部署完成后刷新；必要时用 Ctrl + F5 刷新。
- **想使用自己的域名**：当前免费地址已经可用，以后有需要再设置。

## 官方说明

- [创建 GitHub Pages 网站](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
- [配置发布来源](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
