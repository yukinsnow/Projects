# Projects

静态网页，无需安装依赖。入口为 dist/index.html，可部署到任意静态托管平台。

## 添加和修改项目

编辑 `dist/projects.js`，复制一个项目对象。必填字段：id（GitHub 仓库名）、name、en、kind、category、tagline、description、tags、image、visual、caption、features、note。demo 为可选在线体验地址。

kind 支持 new（新项目）、rebuild（重构）、derivative（衍生）；项目类型可随实际情况调整。当前仅 ikaBeat、elaina 明确为重构，Lite Link 为衍生，其余暂按新项目展示。

图片放入 dist/assets，image 填相对路径。visual 支持 cige / ika / screen / net / hardware / screen lite。普通截图推荐 screen。caption 用于注明图片来源与类型。现有图片均来自对应公开仓库，具体权利与许可遵循原仓库；ikaBeat 角色图和 elaina 插画归原权利人。

项目数和区间文案会自动随项目列表更新。页面支持搜索、类型筛选、项目详情弹窗、手机布局及键盘关闭弹窗。

内容根据 2026-10-26 读取的仓库 README 整理，未设置自动同步。

## Cloudflare Pages 部署

连接 GitHub 仓库 `yukinsnow/Projects`，配置：

| 设置 | 值 |
| --- | --- |
| 生产分支 | `main` |
| Framework preset | `None` |
| Build command | `exit 0` |
| Build output directory | `dist` |
| Root directory | 留空（仓库根目录） |

本项目为原生 HTML/CSS/JS，不需要 npm install、环境变量或服务端。保存部署后，后续推送 main 会由 Cloudflare 自动更新。

本地预览可使用任意静态 HTTP 服务，将 dist 设置为站点目录。

## 展示截图

项目封面优先使用真实界面截图，使用 contain 完整展示，详情支持打开原图。词格酱、elaina、LuCI 与 Lite Link 来自原仓库；ikaBeat 截图来自当前源码的本地网页预览（不代表原生平台验收）。NetScope 暂无可用截图，保留原始图标。

