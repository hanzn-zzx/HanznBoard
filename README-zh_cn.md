# 度表
[English README](./README.md)

一个值日表应用

> 本应用部分使用Trae辅助编程，如有不适请忽略。

> 本项目目前还在进行初期准备~~（画饼）~~，实际功能以成品为准。

## 主要功能

- [ ] 值日表展示、编辑
- [ ] 值日表导出
- [ ] ClassIsland联动（轮值班长显示、劳动提醒、自动化接入）
- [ ] 澜山桌面联动（值周表桌面组件）
- [ ] SecScore联动（轮值班长权限、劳动加减分）

## 技术栈

- 前端：Vue 3 + TypeScript + Vite
- 后端：Tauri + Rust

## 开发与构建

### 开发环境

本项目使用 npm 进行依赖管理。需要安装以下环境：

- [VS Code](https://code.visualstudio.com/) + [Vue - Official](https://marketplace.visualstudio.com/items?itemName=Vue.volar) + [Tauri](https://marketplace.visualstudio.com/items?itemName=tauri-apps.tauri-vscode) + [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)
- [gcc](https://gcc.gnu.org/)（Linux）或 [MSVC](https://visualstudio.microsoft.com/zh-hans/downloads/#build-tools-for-visual-studio-2022)（Windows）
- [Rust](https://www.rust-lang.org/tools/install)（一般自动包含cargo）
- [Node.js](https://nodejs.org/)（一般自动包含npm）

### 开发流程

1. **安装依赖**
```bash
npm install
```

2. **启动开发服务器**
```bash
npm run tauri dev
```

3. **构建生产版本**
```bash
npm run tauri build
```

## 项目结构

```
DutyNote/
├── src/                    # Vue 前端源代码
│   ├── App.vue            # 主应用组件
│   ├── main.ts            # 前端入口文件
│   └── style.css          # 全局样式
├── src-tauri/             # Tauri/Rust 后端
│   ├── src/
│   │   ├── lib.rs        # 库入口（Tauri 命令）
│   │   └── main.rs       # 主程序入口
│   ├── Cargo.toml        # Rust 依赖配置
│   └── tauri.conf.json   # Tauri 配置文件
├── package.json           # Node.js 依赖配置
└── vite.config.ts         # Vite 构建配置
```

## 常用命令

| 命令 | 说明 |
|------|------|
| `npm run dev` | 启动前端开发服务器 |
| `npm run build` | 构建前端生产版本 |
| `npm run tauri dev` | 启动完整的 Tauri 开发环境 |
| `npm run tauri build` | 构建桌面应用安装包 |

## 许可证

GNU GENERAL PUBLIC LICENSE Version 3
