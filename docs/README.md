 # OpenCut 中文文档

 > 本文档翻译自 [OpenCut 官方 README](https://github.com/OpenCut-app/OpenCut/blob/main/README.md)
 > 最后更新：2026-06-23

 ## 关于 OpenCut

 OpenCut 是一个免费、开源的视频编辑器，支持 Web、桌面和移动端。

 ## 项目状态

 **OpenCut 正在从零开始重写。** 新版将带来：

 - **编辑器 API** — 可编程的视频编辑接口
 - **插件系统** — 第三方插件作为一等公民
 - **一套代码，全平台运行** — 基于 Rust 核心，覆盖桌面、移动端和浏览器
 - **MCP 服务器** — 供 AI 智能体调用
 - **无头模式** — 自动化、批量渲染
 - **编辑器内嵌脚本面板** — 直接在编辑器中编写和运行脚本

 你仍然可以在 [opencut-app/opencut-classic](https://github.com/opencut-app/opencut-classic) 找到旧版本，这也是目前可以使用的版本。[opencut.app](https://opencut.app) 目前运行的是 classic 版本；重写版本将先在 [new.opencut.app](https://new.opencut.app) 上线，直到准备好替代旧版。

 ## 本地开发

 首先安装 [proto](https://moonrepo.dev/proto)（如果还没有）：

 ```sh
 bash <(curl -fsSL https://moonrepo.dev/install/proto.sh)
 ```

 在项目根目录下：

 ```sh
 proto use    # 安装 .prototools 中指定的 bun + moon 版本
 bun install
 ```

 启动开发服务器：

 ```sh
 moon run web:dev   # 前端 → localhost:5173
 moon run api:dev   # 后端 → localhost:8787
 ```

 ## 参与贡献

 目前架构还在设计中，暂未开放外部贡献。如果你想关注进展、提问或交流，可以：

 - [加入 Discord](https://discord.gg/zmR9N35cjK)
 - [提交 Issue](https://github.com/opencut-app/opencut/issues)

 ## 赞助商

 OpenCut 得到了相信开源创作工具的公司支持。

 - [**fal.ai**](https://fal.ai)：生成式图像、视频和音频模型，一站式平台。

 想让你的 Logo 出现在这里？联系 [sponsor@opencut.app](mailto:sponsor@opencut.app)。

 ## 开源协议

 [MIT](https://github.com/OpenCut-app/OpenCut/blob/main/LICENSE)
