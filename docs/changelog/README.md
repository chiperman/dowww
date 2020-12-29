---
sidebar: auto
---

# 更新日志

## [1.3.1] - 2020-9-3

### Features

小版本更新，将所有 outdated 信息进行了更新：

- 更新了 WSL 2 的 Windows 10 系统版本要求。
- 更新了 Fluent Terminal 的安装方式，新增了 Fluent Terminal 在 Microsoft Store 微软商店的下载链接。
- 新增了 WSL 2 设置 Git 代理、ssh 登录 GitHub 代理以及自动化配置脚本的方法。
- 新增了 WSL 使用 GPG 对 Git commit 进行签名的方法和问题排查方法。
- 拆分第二章部分内容，将 CLI 命令行工具单独拆为一章。
- 将 Python 环境管理工具由 `pipenv` 改为更加优秀的 Poetry。
- 将 Node.js 版本管理工具由 `nvm` 改为更为先进的 `n`，重构了 Node.js 部分的文档。

为了提升体验：

- 将图片存储更改为阿里云香港 OSS。
- 将图片 CDN 更改为阿里云全球 CDN。

## [1.3.0] - 2020-9-2

### Features

- 移除了全部无用的 CSS 代码，使用 `vuepress-theme-book` 构建文档。
- 抛弃了以版本号更新文档的策略，使用滚动更新策略更新文档。
- 添加自定义滚动条。
- 新增了 WSL 2 中连接 USB 设备的方法。

### Bug fixes

- 更新了全部依赖。
- 移除了脚注构建插件，使用 `markdown-it-footnote` 插件构建脚注。

## [1.2.0] - 2020-7-25

将从 1.1 版本开始陆续新增的 PR 和改动进行了整合，达到 1.2 版本。

### Features

- 新增了关于 WSL 2 配置文件 `.wslconfig` 的说明：[配置 WSL 2 全局选项](https://dowww.spencerwoo.com/4-advanced/4-3-wslconfig.html)。
- 新增了关于重启 WSL 的提示和方法（为了让 WSL 重新挂载 `/mnt` 下的盘符）：[🔁 重启 WSL 环境](https://dowww.spencerwoo.com/2-cli/2-2-shell.html#%E8%A7%A3%E5%86%B3-ls-%E5%91%BD%E4%BB%A4%E8%83%8C%E6%99%AF%E8%89%B2%E9%97%AE%E9%A2%98)。
- 新增了全新的 README 头图 Banner。
- 重新设计了全新的 Dev on Win with WSL 图标。

### Bug fixes

- 修改了 APT 包管理工具的称谓（`Ubuntu` -> `Debian`）。
- 修改了有关 Windows Hyper-V 虚拟机的具体称谓（`已安装的虚拟机平台` -> `虚拟机平台`）。
- 修复了在 Netlify 平台部署时路径大小写不匹配导致无法通过侧边栏导航的问题，错误复盘：[Netlify or VuePress：大型悬疑推理篇之——报错到底是谁的锅？](https://blog.spencerwoo.com/2020/05/debugging-netlify-static-site/)。
- 修改若干错别字（[#59](https://github.com/spencerwooo/dowww/pull/59)）。

## [1.1.0] - 2020-4-15

将从 1.0 版本开始陆续新增的 PR 和改动进行了整合，达到 1.1 版本。

### Features

- 新增了 WSL 2 IP 地址需要手动修改的注意事项：[WSL 2 中的网络访问问题](https://dowww.spencerwoo.com/2-CLI/2-3-Others.html#wsl-2-%E4%B8%AD%E7%9A%84%E7%BD%91%E7%BB%9C%E8%AE%BF%E9%97%AE%E9%97%AE%E9%A2%98)（Issue #49）。
- 新增了 WSL 2 虚拟磁盘空间优化的建议：[优化 WSL 2 虚拟磁盘占用空间](https://dowww.spencerwoo.com/2-CLI/2-3-Others.html#%E4%BC%98%E5%8C%96-wsl-2-%E8%99%9A%E6%8B%9F%E7%A3%81%E7%9B%98%E5%8D%A0%E7%94%A8%E7%A9%BA%E9%97%B4)（PR #45）。
- 新增了 GitHub Sponsors 和爱发电链接，~~请给我打钱！~~（不是）。

### Bugs and fixes

- 修复了 GitHub 主页 README 支付宝二维码失效的问题。
- 修复了 Hyper 终端介绍链接失效的问题：[终端 Terminal - Hyper](https://dowww.spencerwoo.com/2-CLI/2-1-Terminal.html#hyper)。

## [1.0.0] - 2020-1-7 🎉🎉🎉

我们终于迎来了 v1.0.0 的里程碑！文档重构完成，重大更新。历经一周有余，文档几乎全新开始。感谢大家的期待 (✿◡‿◡)

### Features

- 将 VuePress 更新到 1.0 版本，增加了自定义容器和 Medium 风格图片显示。
- 全新的文档色彩方案和设计，使用 [Pantone 2020 Color of the Year](https://time.com/5744039/pantone-color-of-the-year-2020/) 作为强调色。
- 使用更为清晰的侧边栏导航，抛弃使用 navbar 导航栏进行文档导航。
- 在 VuePress 默认主题的基础之上，实现了版本切换、版本归档（`yarn bump-version <VERSION_NUMBER>`）。
- 全新设计了每个部分的「题图」banner，统一设计风格。
- 新增了 WSL 序论、安装部分：
  - 新增了 [关于 WSL、WSL 2 架构设计的介绍](https://dowww.spencerwoo.com/1-Preparations/1-0-Intro.html)。
  - 新增了 [关于 WSL、WSL 2 安装的方法介绍](https://dowww.spencerwoo.com/1-Preparations/1-1-Installation.html)。
- 新增了 CLI 命令行环境中其他工具的配置：
  - 新增了远程登录的配置：[SSH、Mosh 工具的使用](https://dowww.spencerwoo.com/2-CLI/2-3-Others.html#%E8%BF%9C%E7%A8%8B%E7%99%BB%E5%BD%95)。
  - 新增了 [Windows 和 WSL 之间互相文件访问、互相执行命令的方法](https://dowww.spencerwoo.com/2-CLI/2-3-Others.html#windows-%E5%92%8C-wsl-%E4%B9%8B%E9%97%B4%E4%BA%92%E7%9B%B8%E8%AE%BF%E9%97%AE)。

### Changes

- 文档部署到 Netlify，加速中国用户访问。
- 修改了「工具链」部分，将用词切换为「命令行环境 CLI」，更为恰当。
- 修改了 [终端工具 Terminal 环境的配置](https://dowww.spencerwoo.com/2-CLI/2-1-Terminal.html)。
- 修改了 [命令行工具 Shell 环境的配置](https://dowww.spencerwoo.com/2-CLI/2-2-Shell.html)。
- 更新了 VS Code 和 WSL 配合开发的方法：
  - 更新了 [VS Code 远程开发组件包的配置手段](https://dowww.spencerwoo.com/3-VSCode/3-1-Remote-Dev.html)。
  - 更新了 [VS Code 使用 Code Runner 一键执行代码文件的配置](https://dowww.spencerwoo.com/3-VSCode/3-2-Code-Runner.html)。
  - 更新了 [VS Code 连接 WSL 环境开发 Python 项目的配置方法](https://dowww.spencerwoo.com/3-VSCode/3-3-Python.html)。
  - 更新了 [VS Code 连接 WSL 环境开发 C、C++ 项目的配置方法](https://dowww.spencerwoo.com/3-VSCode/3-4-C_Cpp.html)。
  - 更新了 [VS Code 连接 WSL 环境开发 Node.js 项目的配置方法](https://dowww.spencerwoo.com/3-VSCode/3-6-NodeJS.html)。
  - 更新了 [VS Code 连接 WSL 环境撰写 LaTeX 文档的配置方法](https://dowww.spencerwoo.com/3-VSCode/3-5-LaTeX.html)。
- 修改了 [体验、参考、后记](https://dowww.spencerwoo.com/5-Experience/5-0-Intro.html)。

### Removed / Fixed

删除的部分大多数为 Remote 开发组件出现之前，将 VS Code 通过「魔改」的方法与 WSL 环境连接的一些奇淫巧计。不一一赘述。

---

<details>
<summary>Dev on Windows with WSL v0.9 旧版本更新日志</summary>

## [0.2.0] - 2019-12-30

- 开始重构。

## [0.1.1] - 2019-5-13

- 新增了 [Remote-WSL](https://dowww.spencerwoo.com/3-VSCode/#remote-wsl-%E6%8F%92%E4%BB%B6) 更加详细的介绍。

## [0.1.0] - 2019-5-12

- 新增了对 [Windows Terminal](https://dowww.spencerwoo.com/2-Toolchain/2-1-TerminalEnv.html#windows-terminal) 和 [Fluent Terminal](https://dowww.spencerwoo.com/2-Toolchain/2-1-TerminalEnv.html#fluent-terminal) 的介绍。
- 新增了 VS Code [Remote-WSL 支持的介绍](https://dowww.spencerwoo.com/3-VSCode/3-0-Terminal.html#remote-wsl-%E6%8F%92%E4%BB%B6)。
- 新增了 Arch Linux 上架微软官方商店的介绍。

## [0.0.7] - 2019-3-3

### Add

- 新增了 [.NET Core 的配置](https://dowww.spencerwoo.com/3-VSCode/3-7-DotNetCore.html)，[PR #21](https://github.com/spencerwooo/dowww/pull/21)。

## [0.0.6] - 2019-1-24

### Add

- 新增了进阶操作 - [LxRunOffline 的使用配置](https://dowww.spencerwoo.com/4-Advanced/4-2-LxRunOffline.html)，[PR #18](https://github.com/spencerwooo/dowww/pull/18)。
- 新增了 [对 Windows 默认终端模拟器的配置](https://dowww.spencerwoo.com/2-Toolchain/2-1-TerminalEnv.html#%E9%BB%98%E8%AE%A4%E7%9A%84-wsl-%E7%BB%88%E7%AB%AF%E6%A8%A1%E6%8B%9F%E5%99%A8)。

## [0.0.5] - 2019-1-3

### Changed

- 更新了 [VSCode 参考配置内容](https://dowww.spencerwoo.com/3-VSCode/#%E5%8F%82%E8%80%83%E9%85%8D%E7%BD%AE)。
- 完善了 C/Cpp 部分的环境配置指南。
- 更新了 C/Cpp 部分的配图。

## [0.0.4] - 2018-12-30

### Add

- 新增了 [ESLint 的配置](https://dowww.spencerwoo.com/3-VSCode/3-6-NodeJS.html#配置-eslint)。

### Fixed
- 完善了 [Node.js 调试的配置](https://dowww.spencerwoo.com/3-VSCode/3-6-NodeJS.html#调试-node-js-程序)。
- 完善了各部分作者的信息。

## [0.0.3] - 2018-12-26

### Add

- 新增了 [`wslgit` 的加速方法指南](https://dowww.spencerwoo.com/3-VSCode/3-1-Git.html#提升-git-on-wsl-的性能)。
- 新增了 [ArchWSL 入教指南](https://dowww.spencerwoo.com/3-VSCode/3-1-Git.html#提升-git-on-wsl-的性能)。

## [0.0.2] - 2018-12-22

### Add

- 增加了 VSCode 中 Node.js 环境的配置，[PR #11](https://github.com/spencerwooo/dowww/pull/11)。

## [0.0.1] - 2018-12-13

### Add

- 新增了 Terminus 终端的推荐。
- 增加了 VSCode 中 LaTeX 环境的配置，[PR #10](https://github.com/spencerwooo/dowww/pull/10)。


</details>
