# xdoc-feedback

[English](README.md) | **简体中文**

这里用于反馈 `@s8fy/*` npm 包及 Xdoc CLI 的使用问题、兼容性问题和功能建议。

## npm 包概览

| 包                         | 用途                                                                                                                                                |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| `@s8fy/xdoc`               | Xdoc CLI 的 npm 包，提供 `xdoc` 命令，用于创建、编辑、检查、转换和校验演示文稿。详见 [PPTX Runtime](https://docs.structurify.io/en/pptx-runtime/)。 |
| `@s8fy/pptx-viewer`        | 浏览器端 PPTX 预览 SDK，提供与框架无关的 Viewer API 和原生 Web Component，支持幻灯片导航、演示及 PDF 导出。                                         |
| `@s8fy/pptx-viewer-react`  | React 适配包，将共享 Viewer 能力接入 React 组件生命周期。                                                                                           |
| `@s8fy/pptx-viewer-vue`    | Vue 3 适配包，在 Vue 应用中嵌入 PPTX 预览。                                                                                                         |
| `@s8fy/pptx-viewer-svelte` | Svelte 适配包，提供预览所需的 actions 和辅助方法。                                                                                                  |
| `@s8fy/pptx-viewer-solid`  | SolidJS 适配包，在 Solid 应用中使用共享 Viewer 能力。                                                                                               |
| `@s8fy/pptx-converter`     | 独立的 PPTX 转换 SDK，在浏览器、Node.js、Bun 和 Deno 中通过 WebAssembly 本地生成 PDF 或结构化 Markdown，并返回相关图片资源。                        |
| `@s8fy/pptx-parser`        | 底层 PPTX 解析库，提供 JavaScript 和 WebAssembly 双引擎，将演示文稿解析为结构化数据。                                                               |
| `@s8fy/pptx-core`          | 共享核心层，提供统一的演示文稿模型、解析适配、字体与资源生命周期管理，以及 PDF 导出辅助能力。                                                       |
| `@s8fy/pptx-renderer`      | 与框架无关的 DOM/SVG 渲染器及 Viewer 控制器，将演示文稿模型渲染到浏览器。                                                                           |
| `@s8fy/emf2svg`            | 零依赖的 TypeScript EMF/WMF 转 SVG 工具，用于处理演示文稿中的相关矢量图形。                                                                         |

需要在网页中预览 PPTX 时，优先选择 Viewer 或对应框架适配包；只需转换 PDF、Markdown 时，选择 Converter；需要自定义解析和渲染流程时，再使用 Parser、Core 和 Renderer。

## Xdoc CLI

`@s8fy/xdoc` 提供面向本地脚本和 AI Agent 的原生命令行工具 `xdoc`。它可以创建和编辑可编辑的 PPTX，检查文稿结构、应用 JSON patch、比较版本，并完成格式转换、资源提取和校验；同时提供 JSON-RPC、MCP 和本地 daemon 接口。

详见 [PPTX Runtime（Xdoc CLI）](https://docs.structurify.io/en/pptx-runtime/)、[快速开始](https://docs.structurify.io/en/pptx-runtime/getting-started/)和[命令参考](https://docs.structurify.io/en/pptx-runtime/commands/)。

## 官方文档

| 入口                                                                              | 内容                                                        |
| --------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| [文档首页](https://docs.structurify.io/en/)                                       | 产品概览及各产品文档入口。                                  |
| [PPTX Viewer](https://docs.structurify.io/en/pptx-viewer/)                        | 浏览器预览 SDK、配置及 API。                                |
| [Viewer 框架集成](https://docs.structurify.io/en/pptx-viewer/frameworks/)         | React、Vue、Svelte 和 Solid 的接入方式。                    |
| [Viewer Web Component](https://docs.structurify.io/en/pptx-viewer/web-component/) | 原生自定义元素的注册与使用方式。                            |
| [PPTX Converter](https://docs.structurify.io/en/pptx-converter/)                  | 本地 PDF、Markdown 转换及运行时接入说明。                   |
| [Converter API](https://docs.structurify.io/en/pptx-converter/api-reference/)     | 转换函数、选项、返回值与错误处理。                          |
| [Xdoc Agent 工作流](https://docs.structurify.io/en/pptx-runtime/agents/)          | 通过 schema、JSON-RPC、MCP 和 daemon 自动化演示文稿工作流。 |
| [llms.txt](https://docs.structurify.io/llms.txt)                                  | 面向 AI 工具的文档索引，包含各页面的 Markdown 入口。        |

## 问题反馈

反馈时请尽量提供包名或 `xdoc` 命令、版本、运行环境、复现步骤，以及预期结果和实际结果。涉及特定文稿时，可附上脱敏后的最小示例文件和相关截图或错误日志。
