# [0005. egg-bin](https://github.com/Tdahuyou/TNotes.egg/tree/main/notes/0005.%20egg-bin)

<!-- region:toc -->
- [1. 🔗 egg-bin 的 Github 仓库链接](#1--egg-bin-的-github-仓库链接)
- [2. 📒 4.1. 功能](#2--41-功能)
- [3. 📒 4.2. 主要用途](#3--42-主要用途)
- [4. 📒 4.3. 安装方式](#4--43-安装方式)
- [5. 📒 4.4. 使用示例](#5--44-使用示例)
- [6. 📒 4.5. 适用场景](#6--45-适用场景)
<!-- endregion:toc -->

## 1. 🔗 egg-bin 的 Github 仓库链接

- https://github.com/eggjs/bin

## 2. 📒 4.1. 功能

`egg-bin` 是一个开发和调试工具，主要用于本地开发、测试和运行 Egg.js 应用程序。它是 Egg.js 官方提供的 CLI 工具，集成在项目中，而不是全局安装。

## 3. 📒 4.2. 主要用途

- 启动开发服务器（支持热更新）。
- 运行单元测试和覆盖率分析。
- 调试应用（支持断点调试）。
- 执行自定义脚本。

## 4. 📒 4.3. 安装方式

`egg-bin` 通常作为项目的开发依赖安装，而不是全局工具。在使用 `egg-init` 创建项目时，`egg-bin` 会自动被添加到 `devDependencies` 中。

如果你需要手动安装，可以运行：

```bash
npm install egg-bin --save-dev
```

## 5. 📒 4.4. 使用示例

在 `package.json` 中，`egg-bin` 通常会被配置为 npm 脚本。例如：

```json
{
  "scripts": {
    "dev": "egg-bin dev",
    "debug": "egg-bin debug",
    "test": "egg-bin test",
    "cov": "egg-bin cov"
  }
}
```

```bash
# 启动 - 启动开发服务器。（支持热更新）
npm run dev

# 调试 - 启动调试模式，支持断点调试。
npm run debug

# 测试 - 运行单测
npm run test

# 报告 - 运行测试并生成覆盖率报告。
npm run cov
```

## 6. 📒 4.5. 适用场景

- 本地开发和调试。
- 编写和运行单元测试。
- 分析代码覆盖率。
- 需要在开发环境中快速验证功能。
