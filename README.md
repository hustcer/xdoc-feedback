# xdoc-feedback

[**English**](README.md) | [简体中文](README.zh.md)

This repository is the place to report issues, discuss compatibility, and suggest features for the `@s8fy/*` npm packages and Xdoc CLI.

## npm packages

| Package                    | Purpose                                                                                                                                                                                 |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `@s8fy/xdoc`               | npm package for Xdoc CLI, providing the `xdoc` command to create, edit, inspect, convert, and validate presentations. See [PPTX Runtime](https://docs.structurify.io/en/pptx-runtime/). |
| `@s8fy/pptx-viewer`        | Browser PPTX viewer SDK with a framework-neutral API and native Web Component, supporting slide navigation, presentation mode, and PDF export.                                          |
| `@s8fy/pptx-viewer-react`  | React adapter that integrates the shared viewer with the React component lifecycle.                                                                                                     |
| `@s8fy/pptx-viewer-vue`    | Vue 3 adapter for embedding PPTX previews in Vue applications.                                                                                                                          |
| `@s8fy/pptx-viewer-svelte` | Svelte adapter providing viewer actions and helpers.                                                                                                                                    |
| `@s8fy/pptx-viewer-solid`  | SolidJS adapter for using the shared viewer in Solid applications.                                                                                                                      |
| `@s8fy/pptx-converter`     | Standalone SDK that uses WebAssembly to convert PPTX locally to PDF or structured Markdown, returning related image assets, in browsers, Node.js, Bun, and Deno.                        |
| `@s8fy/pptx-parser`        | Low-level PPTX parser with JavaScript and WebAssembly engines that turn presentations into structured data.                                                                             |
| `@s8fy/pptx-core`          | Shared presentation model, parsing adapters, font and resource lifecycle management, and PDF export helpers.                                                                            |
| `@s8fy/pptx-renderer`      | Framework-neutral DOM/SVG renderer and viewer controller for displaying presentation models in the browser.                                                                             |
| `@s8fy/emf2svg`            | Zero-dependency TypeScript EMF/WMF-to-SVG converter for vector graphics embedded in presentations.                                                                                      |

For PPTX previews on the web, start with Viewer or the adapter for your framework. For PDF or Markdown conversion, use Converter. Choose Parser, Core, and Renderer when building a custom parsing or rendering workflow.

## Xdoc CLI

`@s8fy/xdoc` provides `xdoc`, a native command-line tool for local scripts and AI agents. It creates and edits editable PPTX files, inspects presentation structure, applies JSON patches, compares revisions, and handles conversion, resource extraction, and validation. It also exposes JSON-RPC, MCP, and a local daemon.

See [PPTX Runtime (Xdoc CLI)](https://docs.structurify.io/en/pptx-runtime/), [Getting started](https://docs.structurify.io/en/pptx-runtime/getting-started/), and the [Command reference](https://docs.structurify.io/en/pptx-runtime/commands/).

## Documentation

| Resource                                                                                | Contents                                                                         |
| --------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| [Documentation home](https://docs.structurify.io/en/)                                   | Product overview and documentation entry points.                                 |
| [PPTX Viewer](https://docs.structurify.io/en/pptx-viewer/)                              | Browser viewer SDK, configuration, and APIs.                                     |
| [Viewer framework integrations](https://docs.structurify.io/en/pptx-viewer/frameworks/) | Integration with React, Vue, Svelte, and Solid.                                  |
| [Viewer Web Component](https://docs.structurify.io/en/pptx-viewer/web-component/)       | Registering and using the native custom element.                                 |
| [PPTX Converter](https://docs.structurify.io/en/pptx-converter/)                        | Local PDF and Markdown conversion and runtime setup.                             |
| [Converter API](https://docs.structurify.io/en/pptx-converter/api-reference/)           | Conversion functions, options, return values, and error handling.                |
| [Xdoc agent workflows](https://docs.structurify.io/en/pptx-runtime/agents/)             | Presentation automation through schemas, JSON-RPC, MCP, and the daemon.          |
| [llms.txt](https://docs.structurify.io/llms.txt)                                        | Documentation index for AI tools, including Markdown entry points for each page. |

## Reporting issues

Please include the package name or `xdoc` command, version, runtime environment, steps to reproduce, and expected and actual results. For document-specific issues, attach a minimal sample with sensitive information removed, along with relevant screenshots or error logs.
