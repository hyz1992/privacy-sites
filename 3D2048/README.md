# 隐私保护指引静态网页

按 SUD 提供的《用户隐私保护指引设置.docx》固定章节整理，不新增广告专章。三个语言版本为同一内容的对应翻译；保留原模板的共享、披露与保存期限条款。游戏名沿用工程 `assets/scripts/GameBrand.ts`：中文“3D叠叠乐”、英文“Bump & Double”、俄语“Кубики ×2”。

## 文件

- `index.html`：中文版。
- `en.html`：英文版。
- `ru.html`：俄语版。
- `style.css`：共用样式。
- `.nojekyll`：告知 GitHub Pages 直接发布静态文件。

纯静态 HTML/CSS，无构建、JavaScript、在线字体、表单或追踪脚本。双击 `index.html` 也可离线查看和切换语言。

## 已填写的信息

- 开发者：huang yu zhao，按用户提供的原样填写。
- 联系邮箱：huangyz192@gmail.com，两处联系位置均可点击发送邮件。
- 更新日期与生效日期：2026-10-15。

三语页面均无待填占位符。保留原模板的五个主章节，删除空的插件／SDK示例条目，改为简短 SUD 平台服务说明及其官方隐私政策链接；不虚构具体 SDK 名称、提供方或采集范围，也不声明未使用第三方服务。具体 SDK 清单及平台审核适用性未核实，本网页不代表平台已经审核通过。

原模板中收集昵称、头像、性别、地区、手机号、身份证号的示例，没有作为事实照抄。开发者处理信息一节按当前实现写入本地存档、设置与本地统计，不将本地随机标识称为完全匿名；“不自动上传”仅限定于游戏自身的本地统计，不涵盖第三方服务。正式接入改变实际处理行为时，应同步修订三语对应段落。

原模板“存储在中国大陆”标注仅境外主体需要填写，因此未默认加入该句；若该条件适用，应根据真实存储情况补充。撤回授权使用联系邮箱及相应平台权限管理的一般说明，没有编造固定菜单路径。

文件可直接作为静态站点上传。网页展示本身不会实现游戏内授权或撤回功能。英文、俄语沿用原文的中国法语境，不额外声称满足其他司法辖区的全部要求。

## GitHub Pages 部署

最简单的方式是创建独立的 GitHub 仓库，将本目录的三个 HTML、`style.css` 和 `.nojekyll` 放在仓库根目录，保留相对位置。可同时放入本 README；上传时不要漏掉以点开头的 `.nojekyll`。

在仓库 `Settings → Pages → Build and deployment` 中选择 `Deploy from a branch`，选择实际分支（例如 `main`）和 `/(root)`，保存后等待部署完成。

假设仓库名为 `game-privacy`，发布地址为：

- 中文：`https://你的用户名.github.io/game-privacy/`
- 英文：`https://你的用户名.github.io/game-privacy/en.html`
- 俄语：`https://你的用户名.github.io/game-privacy/ru.html`

资源和语言链接均使用相对路径，支持 GitHub Pages 项目子目录。无需安装依赖或上传游戏工程。若改用现有 Pages 仓库，把三个 HTML 和 CSS 放在其已发布目录内的同一子目录即可；`.nojekyll` 放在该站点的发布源根目录。不能直接选择 `docs/privacy-policy` 作为分支发布源目录。

## 维护参考

- 结构来源：用户提供的 SUD《用户隐私保护指引设置.docx》。
- [SUD 小游戏隐私合规开发指南](https://developer.sud.tech/openpaas/minigame/introduction/minigame-integration-guide/privacy/user-privacy-protection.html)。
- [GitHub Pages 发布源设置](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。

## TapTap 小游戏专用版本

- 源文件：[`taptap/index.html`](taptap/index.html)，复用上级 `style.css`。
- GitHub Pages：<https://hyz1992.github.io/privacy-sites/3D2048/taptap/>。
- 适用《方糖叠叠乐》Tap 小游戏 0.1.2，说明本地存档、设备适配和平台服务；不复用 Android APK 的广告 SDK 条款。
- 修改源码并发布后，核对上述公开地址，再将其填入 TapTap 后台隐私政策链接。当前目录根部的中英俄页面仍用于原 SUD 版本。
